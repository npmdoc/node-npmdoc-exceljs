# api documentation for  [exceljs (v0.4.2)](https://github.com/guyonroche/exceljs#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-exceljs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-exceljs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-exceljs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-exceljs)
#### Excel Workbook Manager - Read and Write xlsx and csv Files.

[![NPM](https://nodei.co/npm/exceljs.png?downloads=true)](https://www.npmjs.com/package/exceljs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-exceljs/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-exceljs_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-exceljs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-exceljs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-exceljs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Guyon Roche"
    },
    "bugs": {
        "url": "https://github.com/guyonroche/exceljs/issues"
    },
    "dependencies": {
        "archiver": "^1.3.0",
        "fast-csv": "^2.4.0",
        "jszip": "3.1.3",
        "moment": "^2.17.1",
        "promish": ">=5.0.2",
        "sax": "^1.2.2",
        "unzip2": "^0.2.5"
    },
    "description": "Excel Workbook Manager - Read and Write xlsx and csv Files.",
    "devDependencies": {
        "babel-polyfill": "^6.23.0",
        "babel-preset-es2015": "^6.22.0",
        "bluebird": "^3.4.7",
        "browserify": "^14.1.0",
        "chai": "*",
        "chai-datetime": "*",
        "chai-xml": "*",
        "express": "*",
        "grunt": "^1.0.1",
        "grunt-babel": "^6.0.0",
        "grunt-browserify": "^5.0.0",
        "grunt-contrib-jasmine": "^1.1.0",
        "grunt-contrib-uglify": "^2.1.0",
        "grunt-contrib-watch": "^1.0.0",
        "jshint": "*",
        "memorystream": "*",
        "mocha": "*",
        "request": "*",
        "uglifyjs": "^2.4.10",
        "underscore": "^1.8.3"
    },
    "directories": {},
    "dist": {
        "shasum": "7f310befe11efa1a781f74f15359d74b8c12c66b",
        "tarball": "https://registry.npmjs.org/exceljs/-/exceljs-0.4.2.tgz"
    },
    "files": [
        "excel.js",
        "lib",
        "dist",
        "LICENSE",
        "README.md",
        "MODEL.md"
    ],
    "gitHead": "33e3db85359861834dfea5105a9f26a19ac50325",
    "homepage": "https://github.com/guyonroche/exceljs#readme",
    "keywords": [
        "xlsx",
        "json",
        "csv",
        "excel",
        "font",
        "border",
        "fill",
        "number",
        "format",
        "number format",
        "alignment",
        "office",
        "spreadsheet",
        "workbook",
        "defined names",
        "data validations",
        "rich text",
        "in-cell format",
        "outlineLevel",
        "views",
        "frozen",
        "split",
        "pageSetup"
    ],
    "license": "MIT",
    "main": "./excel.js",
    "maintainers": [
        {
            "name": "guyonroche",
            "email": "cyber.sapiens@hotmail.com"
        }
    ],
    "name": "exceljs",
    "optionalDependencies": {},
    "private": false,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/guyonroche/exceljs.git"
    },
    "scripts": {
        "browser-test": "grunt jasmine",
        "build": "grunt build",
        "clean": "rm -rf build/ && rm -rf dist",
        "clean-build": "npm run clean && npm run build",
        "end-to-end-test": "mocha spec/end-to-end --recursive",
        "integration-test": "mocha spec/integration --recursive",
        "manual-test": "node spec/manual/app.js",
        "prepublish": "npm run build && npm test",
        "test": "npm run unit-test && npm run integration-test && npm run end-to-end-test && npm run browser-test",
        "unit-test": "mocha spec/unit --recursive"
    },
    "version": "0.4.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module exceljs](#apidoc.module.exceljs)
1.  [function <span class="apidocSignatureSpan">exceljs.</span>ModelContainer (model)](#apidoc.element.exceljs.ModelContainer)
1.  [function <span class="apidocSignatureSpan">exceljs.</span>Workbook ()](#apidoc.element.exceljs.Workbook)
1.  object <span class="apidocSignatureSpan">exceljs.</span>DocumentType
1.  object <span class="apidocSignatureSpan">exceljs.</span>ErrorValue
1.  object <span class="apidocSignatureSpan">exceljs.</span>ReadingOrder
1.  object <span class="apidocSignatureSpan">exceljs.</span>RelationshipType
1.  object <span class="apidocSignatureSpan">exceljs.</span>ValueType
1.  object <span class="apidocSignatureSpan">exceljs.</span>Workbook.prototype
1.  object <span class="apidocSignatureSpan">exceljs.</span>config
1.  object <span class="apidocSignatureSpan">exceljs.</span>exceljs_browser
1.  object <span class="apidocSignatureSpan">exceljs.</span>stream

#### [module exceljs.Workbook](#apidoc.module.exceljs.Workbook)
1.  [function <span class="apidocSignatureSpan">exceljs.</span>Workbook ()](#apidoc.element.exceljs.Workbook.Workbook)

#### [module exceljs.Workbook.prototype](#apidoc.module.exceljs.Workbook.prototype)
1.  [function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>_removeWorksheet (worksheet)](#apidoc.element.exceljs.Workbook.prototype._removeWorksheet)
1.  [function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>addWorksheet (name, options)](#apidoc.element.exceljs.Workbook.prototype.addWorksheet)
1.  [function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>clearThemes ()](#apidoc.element.exceljs.Workbook.prototype.clearThemes)
1.  [function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>eachSheet (iteratee)](#apidoc.element.exceljs.Workbook.prototype.eachSheet)
1.  [function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>getWorksheet (id)](#apidoc.element.exceljs.Workbook.prototype.getWorksheet)
1.  [function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>removeWorksheet (id)](#apidoc.element.exceljs.Workbook.prototype.removeWorksheet)
1.  object <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>_csv
1.  object <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>_xlsx
1.  object <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>csv
1.  object <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>xlsx

#### [module exceljs.config](#apidoc.module.exceljs.config)
1.  [function <span class="apidocSignatureSpan">exceljs.config.</span>setValue (key, value, overwrite)](#apidoc.element.exceljs.config.setValue)

#### [module exceljs.exceljs_browser](#apidoc.module.exceljs.exceljs_browser)
1.  [function <span class="apidocSignatureSpan">exceljs.exceljs_browser.</span>Workbook ()](#apidoc.element.exceljs.exceljs_browser.Workbook)
1.  object <span class="apidocSignatureSpan">exceljs.exceljs_browser.</span>DocumentType
1.  object <span class="apidocSignatureSpan">exceljs.exceljs_browser.</span>ErrorValue
1.  object <span class="apidocSignatureSpan">exceljs.exceljs_browser.</span>ReadingOrder
1.  object <span class="apidocSignatureSpan">exceljs.exceljs_browser.</span>RelationshipType
1.  object <span class="apidocSignatureSpan">exceljs.exceljs_browser.</span>ValueType



# <a name="apidoc.module.exceljs"></a>[module exceljs](#apidoc.module.exceljs)

#### <a name="apidoc.element.exceljs.ModelContainer"></a>[function <span class="apidocSignatureSpan">exceljs.</span>ModelContainer (model)](#apidoc.element.exceljs.ModelContainer)
- description and source-code
```javascript
ModelContainer = function (model) {
  this.model = model;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.exceljs.Workbook"></a>[function <span class="apidocSignatureSpan">exceljs.</span>Workbook ()](#apidoc.element.exceljs.Workbook)
- description and source-code
```javascript
Workbook = function () {
  this.created = new Date();
  this.modified = this.created;
  this.properties = {};
  this._worksheets = [];
  this.views = [];
  this._definedNames = new DefinedNames();
}
```
- example usage
```shell
...
'''javascript
var Excel = require('exceljs');
'''

## Create a Workbook

'''javascript
var workbook = new Excel.Workbook();
'''

## Set Workbook Properties

'''javascript
workbook.creator = 'Me';
workbook.lastModifiedBy = 'Her';
...
```



# <a name="apidoc.module.exceljs.Workbook"></a>[module exceljs.Workbook](#apidoc.module.exceljs.Workbook)

#### <a name="apidoc.element.exceljs.Workbook.Workbook"></a>[function <span class="apidocSignatureSpan">exceljs.</span>Workbook ()](#apidoc.element.exceljs.Workbook.Workbook)
- description and source-code
```javascript
Workbook = function () {
  this.created = new Date();
  this.modified = this.created;
  this.properties = {};
  this._worksheets = [];
  this.views = [];
  this._definedNames = new DefinedNames();
}
```
- example usage
```shell
...
'''javascript
var Excel = require('exceljs');
'''

## Create a Workbook

'''javascript
var workbook = new Excel.Workbook();
'''

## Set Workbook Properties

'''javascript
workbook.creator = 'Me';
workbook.lastModifiedBy = 'Her';
...
```



# <a name="apidoc.module.exceljs.Workbook.prototype"></a>[module exceljs.Workbook.prototype](#apidoc.module.exceljs.Workbook.prototype)

#### <a name="apidoc.element.exceljs.Workbook.prototype._removeWorksheet"></a>[function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>_removeWorksheet (worksheet)](#apidoc.element.exceljs.Workbook.prototype._removeWorksheet)
- description and source-code
```javascript
_removeWorksheet = function (worksheet) {
  delete this._worksheets[worksheet.id];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.exceljs.Workbook.prototype.addWorksheet"></a>[function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>addWorksheet (name, options)](#apidoc.element.exceljs.Workbook.prototype.addWorksheet)
- description and source-code
```javascript
addWorksheet = function (name, options) {

  var id = this.nextId;
  name = name || 'sheet' + id;

  // if options is a color, call it tabColor (and signal deprecated message)
  if (options) {
    if (typeof options === 'string') {
      console.trace('tabColor argument is now deprecated. Please use workbook.addWorksheet(name, {properties: { tabColor: { argb
: "rbg value" } }');
      options = {
        properties: {
          tabColor: {argb: options}
        }
      };
    } else if (options.argb || options.theme || options.indexed) {
      console.trace('tabColor argument is now deprecated. Please use workbook.addWorksheet(name, {properties: { tabColor: { ... } }');
      options = {
        properties: {
          tabColor: options
        }
      };
    }
  }

  var worksheetOptions = Object.assign({}, options, {
    id: id,
    name: name,
    workbook: this
  });

  var worksheet = new Worksheet(worksheetOptions);

  this._worksheets[id] = worksheet;
  return worksheet;
}
```
- example usage
```shell
...
  }
]
'''

## Add a Worksheet

'''javascript
var sheet = workbook.addWorksheet('My Sheet');
'''

Use the second parameter of the addWorksheet function to specify options for the worksheet.

For Example:

'''javascript
...
```

#### <a name="apidoc.element.exceljs.Workbook.prototype.clearThemes"></a>[function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>clearThemes ()](#apidoc.element.exceljs.Workbook.prototype.clearThemes)
- description and source-code
```javascript
clearThemes = function () {
  // Note: themes are not an exposed feature, meddle at your peril!
  this._themes = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.exceljs.Workbook.prototype.eachSheet"></a>[function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>eachSheet (iteratee)](#apidoc.element.exceljs.Workbook.prototype.eachSheet)
- description and source-code
```javascript
eachSheet = function (iteratee) {
  this._worksheets.forEach(function(sheet) {
    iteratee(sheet, sheet.id);
  });
}
```
- example usage
```shell
...
var sheet = workbook.addWorksheet('My Sheet', {views:[{xSplit: 1, ySplit:1}]});
'''

## Access Worksheets
'''javascript
// Iterate over all sheets
// Note: workbook.worksheets.forEach will still work but this is better
workbook.eachSheet(function(worksheet, sheetId) {
    // ...
});

// fetch sheet by name
var worksheet = workbook.getWorksheet('My Sheet');

// fetch sheet by id
...
```

#### <a name="apidoc.element.exceljs.Workbook.prototype.getWorksheet"></a>[function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>getWorksheet (id)](#apidoc.element.exceljs.Workbook.prototype.getWorksheet)
- description and source-code
```javascript
getWorksheet = function (id) {
  if (id === undefined) {
    return this._worksheets.find(function(worksheet) { return worksheet; });
  } else if (typeof(id) === 'number') {
    return this._worksheets[id];
  } else if (typeof id === 'string') {
    return this._worksheets.find(function(worksheet) {
      return worksheet && worksheet.name == id;
    });
  } else {
    return undefined;
  }
}
```
- example usage
```shell
...
// Iterate over all sheets
// Note: workbook.worksheets.forEach will still work but this is better
workbook.eachSheet(function(worksheet, sheetId) {
    // ...
});

// fetch sheet by name
var worksheet = workbook.getWorksheet('My Sheet');

// fetch sheet by id
var worksheet = workbook.getWorksheet(1);
'''

## Worksheet Properties
...
```

#### <a name="apidoc.element.exceljs.Workbook.prototype.removeWorksheet"></a>[function <span class="apidocSignatureSpan">exceljs.Workbook.prototype.</span>removeWorksheet (id)](#apidoc.element.exceljs.Workbook.prototype.removeWorksheet)
- description and source-code
```javascript
removeWorksheet = function (id) {
  var worksheet = this.getWorksheet(id);
  if (worksheet) {
    worksheet.destroy();
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.exceljs.config"></a>[module exceljs.config](#apidoc.module.exceljs.config)

#### <a name="apidoc.element.exceljs.config.setValue"></a>[function <span class="apidocSignatureSpan">exceljs.config.</span>setValue (key, value, overwrite)](#apidoc.element.exceljs.config.setValue)
- description and source-code
```javascript
function setValue(key, value, overwrite) {
  if (overwrite === undefined) {
    // only avoid overwrite if explicitly disabled
    overwrite = true;
  }
  switch(key.toLowerCase()) {
    case 'promise':
      if (!overwrite && PromishLib.Promish) return;
      PromishLib.Promish = value;
      break;
  }
}
```
- example usage
```shell
...

# Config

ExcelJS now supports dependency injection for the promise library.
 You can restore Bluebird promises by including the following code in your module...

'''javascript
ExcelJS.config.setValue('promise', require('bluebird'));
'''

Please note: I have tested ExcelJS with bluebird specifically (since up until recently this was the library it used).
 From the tests I have done it will not work with Q.

# Known Issues
...
```



# <a name="apidoc.module.exceljs.exceljs_browser"></a>[module exceljs.exceljs_browser](#apidoc.module.exceljs.exceljs_browser)

#### <a name="apidoc.element.exceljs.exceljs_browser.Workbook"></a>[function <span class="apidocSignatureSpan">exceljs.exceljs_browser.</span>Workbook ()](#apidoc.element.exceljs.exceljs_browser.Workbook)
- description and source-code
```javascript
Workbook = function () {
  this.created = new Date();
  this.modified = this.created;
  this.properties = {};
  this._worksheets = [];
  this.views = [];
  this._definedNames = new DefinedNames();
}
```
- example usage
```shell
...
'''javascript
var Excel = require('exceljs');
'''

## Create a Workbook

'''javascript
var workbook = new Excel.Workbook();
'''

## Set Workbook Properties

'''javascript
workbook.creator = 'Me';
workbook.lastModifiedBy = 'Her';
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
