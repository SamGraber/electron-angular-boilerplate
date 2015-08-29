[![Dependency Status](https://david-dm.org/yuki-takei/electron-angular-boilerplate
.svg)](https://david-dm.org/alexweber/electron-angular-boilerplate
) [![devDependency Status](https://david-dm.org/yuki-takei/electron-angular-boilerplate
/dev-status.svg)](https://david-dm.org/yuki-takei/electron-angular-boilerplate#info=devDependencies)

electron-angular-boilerplate
============================


Features
--------

* Electron
  * ES6
* AngularJS 1.x
  * Typescript
* Bootstrap3
* LESS (with less.js when developing)
* LiveReload
* compile and minify for production
  * Electron: Babel and Browserify
  * AngularJS: JSPM
  * LESS to CSS
* package for Windows, Mac OSX, and Linux


Requirements
------------

* node.js  
(confirmed to work with v0.12.7)


Usage
------

### Install dependencies

```
$ cd /path/to/local_repos
$ npm install -g gulp jspm dtsm
$ npm install
$ jspm install
```

### Install DefinitelyTyped files

```
$ dtsm install
```

### Run at local

```
## provides a http server that hosts an angular app run by JSPM
$ gulp serve

## provides a http server that hosts an angular app
##     run with Self-Executing (SFX) Bundles generated by JSPM
$ gulp serve:dist

## privides an electron server that loads an angular app run by JSPM
$ gulp serve:electron

## privides an electron server that loads an angular app
##     run with Self-Executing (SFX) Bundles generated by JSPM
$ gulp serve:dist:electron
```

### Release

```
$ gulp package
```

Directory Structure
-------------------

```
/
├── .tmp
│   ├── dist              # location for compiled Angular2 App files
│   ├── typings           # location for DefinitelyTyped files
│   └── serve             # location for compiled Electron App files
├── gulp                  # gulp tasks
├── src                   # Angular2 Application src dir
│   ├── app               # main module for Angular2 Application
│   ├── index.dev.html    # entry point (development)
│   ├── index.html        # entry point (production)
│   ├── jspm.config.js    # JSPM config file
└── src-electron          # Electron Application src dir
```


Note
-----

A boilerplate with Angular2 ver is [here](https://github.com/yuki-takei/electron-angular2-boilerplate).


Contributing
------------

1. Fork the repository on Github
1. Write your change
1. Submit a Pull Request using Github


License and Authors
-------------------
- Author:: Yuki Takei (<yuki@weseek.co.jp>)

Licensed under the Apache License, Version 2.0 (the "License");  
you may not use this file except in compliance with the License.  
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software  
distributed under the License is distributed on an "AS IS" BASIS,  
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  
See the License for the specific language governing permissions and  
limitations under the License.