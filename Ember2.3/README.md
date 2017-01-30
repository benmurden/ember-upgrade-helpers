## Tests

### Serializer Tests
[`JSONAPIAdapter`][1] is now the default adapter, meaning that if any other adapter was used, unchanged serializer tests will fail with errors like the following.

```
Cannot read property 'replace' of undefined
```

Be sure to include `application:adapter` in your test's `needs` array if you are using anything other than the default adapter, or an adapter that does not directly inherit from [`JSONAPIAdapter`][1].

```js
moduleFor('serializer:foo', 'Integration | Serializer | foo', {
  needs: ['model:foo', 'adapter:application']
});
```

[1]: http://emberjs.com/api/data/classes/DS.JSONAPIAdapter.html