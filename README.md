# Amber
amber is a command line tool to create Sass components and thier responsive files.
it will create a new component and include it inside the _all.scc file also will create 4 Mixin and include them in thier files inside the ( Responsive ) folder.

---

## Requirments:
Node.js (v8.5.0+) [https://nodejs.org/en/]

Git [https://git-scm.com]

Sass [https://sass-lang.com] or you can use anything to compile from sass to css

---

## Usage:
### 1- Clone The Project Files:
```git clone https://github.com/adel-bassiony/amber.git```

### 2- Create New Project ( new sass folder + structure ):

##### Using Node.js:
```node amber/commands/create_structure.js```

##### Using NPM (add this line inside your scripts):
```"cs": "node amber/commands/create_structure.js"```


### 3- Create New Component:

##### Using Node.js:
```node amber/commands/create_component.js```

##### Using NPM (add this line inside your scripts):

```"cc": "node amber/commands/create_component.js"```


### 4- Compile From Sass to CSS (Optional | You can use anything else to compile the sass files):

##### Using Sass:
###### Output the minifed version:
```sass --watch sass/style.scss:css/style.min.css sass/style-rtl.scss:css/style-rtl.min.css --style compressed```
###### Output the unminifed version:
```sass --watch sass/style.scss:css/style.css sass/style-rtl.scss:css/style-rtl.css```

##### Using NPM (add this line inside your scripts):
###### Output the minifed version:
```"sass-min": "sass --watch sass/style.scss:css/style.min.css sass/style-rtl.scss:css/style-rtl.min.css --style compressed"```
###### Output the unminifed version:
```"sass": "sass --watch sass/style.scss:css/style.css sass/style-rtl.scss:css/style-rtl.css"```
