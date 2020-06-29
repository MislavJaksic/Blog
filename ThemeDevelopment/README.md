## Ghost Theme Development

[Install Ghost locally](https://github.com/MislavJaksic/Knowledge-Repository/tree/master/Technology/Web/CMS/Ghost/Docs/Setup/Local)  

```
$: pwd ->  # path with `.ghost-cli`

$: ghost ls
$: ghost start
$: ghost restart
$: ghost stop
```

Visit:
* http://localhost:2368
* http://localhost:2368/ghost

```
Email: jaksicmislav@gmail.com
Password: 0123456789
```

`theme` in `/content/themes/`.  

```
$: gscan custom-casper/content/themes/casper
```

### Tips and Tricks

`ghost restart` after adding a `*.hbs` file.  

`{{!< Handlebar-File-Name}}`: insert self into a `*.hbs` file
`{{{body}}}`: where other `*.hbs` files insert themselves

Link page to URL manually:
```
routes:
  /Http-Path/:
    permalink: /Http-Path/
    template: Handlebar-File-Name
```
