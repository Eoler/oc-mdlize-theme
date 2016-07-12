# Blank-Materialize
A blank theme for [OctoberCMS](https://octobercms.com/) with [Materialize](http://materializecss.com/) framework & [jQuery](https://jquery.com/).


## Installation
`$ php artisan theme:install martin.blank-materialize <theme>`

Replace `<theme>` with the name of your theme.


## Using the theme
`$ php artisan theme:use <name>`

Where `<name>` is whatever you specified in `theme:install`.


## Customize
If you are not planning to use Materialize icons, remove this line: `<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">`

Comment out unwanted component styles / scripts to create custom Materialize library in:
- assets/scss/materialize.scss
- assets/es6/materialize.js

Development changes can be automated with command-line instruction inside *theme root*:
```
gulp watch
```
Build optimized, minified, autoprefixed assets with command-line instruction inside *theme root*:
```
gulp --production
```

## One-time Development Environment Setup
Install [NodeJS and Node Package Manager](https://nodejs.org/en/) globally (Stable version preferred).
Run the following command-line instructions inside *theme root*:
```
npm install --global gulp bower
npm install && bower install
```

