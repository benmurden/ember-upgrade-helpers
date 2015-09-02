## Sublime Text
```
Find:    \{\{\s*#each ([a-zA-Z0-9]+) in ([a-zA-Z0-9\.]+)( itemController="[a-zA-Z0-9_]+")?\s*\}\}
Replace: {{#each \2\3 as |\1|}}
```
## Vim
```
:%s/{{\s*#each ([a-zA-Z0-9]+) in ([a-zA-Z0-9\.]+)( itemController="[a-zA-Z0-9_]+")?\s*}}/{{#each \2\3 as |\1|}}/g
```
