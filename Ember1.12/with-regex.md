## Sublime Text
Find:    \{\{#with ([a-zA-Z0-9_\-\.]*) as ([a-zA-Z0-9]*)\}\}
Replace: {{#with \1 as |\2|}}

## Vim
:%s/{{#with ([a-zA-Z0-9_\-\.]*) as ([a-zA-Z0-9_\-]*)}}/{{#with \1 as |\2|}}
