# Blank-Materialize
Starter development template for building [Materialize](http://materializecss.com/) themed [OctoberCMS](//octobercms.com/) sites.

Includes:
- latest Materialize [source from official Bower repository](https://github.com/Dogfalo/materialize)
- [GulpJS-based build system](https://nystudio107.com/blog/a-gulp-workflow-for-frontend-development-automation) for development and production
- [NPM-based config system](https://nystudio107.com/blog/a-better-package-json-for-the-frontend) for development and production


## Installation
Add the theme to existing project while logged into OctoberCMS account online,
or interactively by searching it inside Settings/System/Updates/Themes in backend,
or with the following command-line instructions inside *project root*:
```
php artisan theme:install castus.mdlize mdlize
php artisan theme:use f5fresh
```

## One-time Development Environment Setup
Install [NodeJS and Node Package Manager](https://nodejs.org/en/) globally (version up to v14.LTS preferred for Gulp ^3).
Run the following command-line instructions inside *theme root*:
```
npm install --global gulp-cli bower
npm install && bower install
```
Integrating build process into OctoberCMS project is easy - copy (or merge into existing) files into *project root*:
```
gulpfile.js
package.json
```
Adjust `paths.root` configuration variable to **themes/castus-mdlize/** and start using command-line tasks from *project root*.

## Using and Editing
Development changes can be automated with command-line instruction from configured Gulpfile (project or theme) *build root*:
```
gulp watch
```
Build versioned, optimized, minified, autoprefixed assets with command-line instruction:
```
gulp upbuild --production
```

