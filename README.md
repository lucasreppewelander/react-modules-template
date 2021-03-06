# React Modules Template
> Easy create new react modules with this tool

## Installation
```
npm install -g react-modules-template
```

## Usage
```
react-module <ComponentName> [--pure]
```

#### Example
```
react-module Login
```

This will generate a Folder named Login relative to your current path
and three files: an empty Login.scss and another file named Login.jsx filled with
starter code for exporting a module with custom css.

If you would like to generate a stateless component you can pass in the `--pure` flag after the componentName, this flag is optional. E.g: `react-module TableRow --pure`, this will generate a pure function with the name of TableRow with a corresponding style file and a test file.

### Get started

Install the package globally and then run the `--init` command below.
```
react-module --init
```

This will step you through some configuration questions to make this package create files according to your project, in this init you can specify javascript extension, css extension and wheter or not to use ES6 classes.

## Changelog

#### v3.1.0
Added the `--pure` flag to generate stateless components.

#### v3.0.0
Changed the main file to be named index.extension instead of componentName.extension, because I hated that I had to import it like this `import component from '/component/component'`.
Now I can only import it like this: `import component from '/component'`

#### v2.0.0
Added functionality for a configuration file, added the `--init` flag when running to create the config file.
Made it easier to customise to your own coding style and file structure.

#### v1.2.0
Added a jest .js test file, the starter code only checks that it can be rendered, but it can be filled with more!

## Output
```
./Login
    --- index.[js|jsx]
    --- Login.test.js
    --- Login.[scss|css]
```
