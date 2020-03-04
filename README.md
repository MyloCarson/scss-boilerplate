> # INTRODUCTION

I orchestrated this scss boilerplate as quick way to implement SCSS in React, Angular or any other framework or library that understands SCSS.

# Usage

> ## Using in basic HTML

## OPTION 1
Install VScode plugin to convert **styles.scss** to **styles.css**

## OPTION 2
Step 1: Install **node-sass** via yarn or npm

``` yarn add node-sass ```

## OR

``` npm install node-sass```

Step 2: Go to **package.json**, paste this,
```
"scripts": {
      "scss": "node-sass --watch assets/scss -o assets/css"
  }
```
NOTE: With this step, as soon as you start adding styles to any of the stylesheets, **styles.scss**  will be recomplied and converted into **styles.css**

> ## Using in React

React now understands .scss. All that is required to do is to import **styles.css** into your **App.js**

> ## Using in Angular

Set up your angular project to use .scss for styling. Then,
* 1: Open **angular.json** located in the root directory of the project
* 2: Add the path **'assets/scss/styles.scss'** to the **styles** node. Like so,

```
{
  "$schema": ".....",
  "version": 1,
  "newProjectRoot": "....",
  "projects": {
    "project-name": {
      .........
      "architect": {
        "build": {
            "styles": [
              "src/styles.scss"
            ],
        }
        ..........
        }
        ....
    }

    ...
  }
  ...
}
```

> # BASIC FOLDER STRUCTURE
- __scss\-boilerplate__
   - [README.md](README.md)
   - __assets__
     - __fonts__
     - __images__
       - __svgs__
     - __scss__
       - __components__
         - [\_button.scss](assets/scss/components/_button.scss)
         - [\_card.scss](assets/scss/components/_card.scss)
         - [\_footer.scss](assets/scss/components/_footer.scss)
         - [\_form.scss](assets/scss/components/_form.scss)
         - [\_header.scss](assets/scss/components/_header.scss)
         - [\_menu.scss](assets/scss/components/_menu.scss)
       - __layouts__
       - [styles.scss](assets/scss/styles.scss)
       - __utils__
         - [\_globals.scss](assets/scss/utils/_globals.scss)
         - [\_settings.scss](assets/scss/utils/_settings.scss)
         - [\_typography.scss](assets/scss/utils/_typography.scss)
