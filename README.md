# api documentation for  [parker (v0.0.10)](https://github.com/katiefenn/parker)  [![npm package](https://img.shields.io/npm/v/npmdoc-parker.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-parker) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-parker.svg)](https://travis-ci.org/npmdoc/node-npmdoc-parker)
#### Stylesheet analysis tool for CSS

[![NPM](https://nodei.co/npm/parker.png?downloads=true)](https://www.npmjs.com/package/parker)

[![apidoc](https://npmdoc.github.io/node-npmdoc-parker/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-parker_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-parker/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-parker/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-parker/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Katie Fenn"
    },
    "bin": {
        "parker": "./parker.js"
    },
    "bugs": {
        "url": "https://github.com/katiefenn/parker/issues"
    },
    "dependencies": {
        "async": "~0.2.10",
        "cli-color": "*",
        "graceful-fs": "~3.0.2",
        "lodash": "^3.2.0",
        "minimist": "0.0.7"
    },
    "description": "Stylesheet analysis tool for CSS",
    "devDependencies": {
        "chai": "*",
        "mocha": "*",
        "sinon": "*",
        "sinon-chai": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "b72604f5e3ced31a2b06128e449670f68dd5dc20",
        "tarball": "https://registry.npmjs.org/parker/-/parker-0.0.10.tgz"
    },
    "gitHead": "9d55993e20c3f6554bae2f958af1997ff8f80bac",
    "homepage": "https://github.com/katiefenn/parker",
    "keywords": [
        "css",
        "stylesheet",
        "analysis"
    ],
    "license": "MIT",
    "main": "parker.js",
    "maintainers": [
        {
            "name": "katiefenn",
            "email": "katie.fenn.parker@gmail.com"
        }
    ],
    "name": "parker",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/katiefenn/parker.git"
    },
    "scripts": {
        "test": "mocha --no-colors --reporter spec"
    },
    "version": "0.0.10"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module parker](#apidoc.module.parker)
1.  [function <span class="apidocSignatureSpan">parker.</span>CliController ()](#apidoc.element.parker.CliController)
1.  [function <span class="apidocSignatureSpan">parker.</span>CliFormatter ()](#apidoc.element.parker.CliFormatter)
1.  [function <span class="apidocSignatureSpan">parker.</span>CssDeclaration (raw)](#apidoc.element.parker.CssDeclaration)
1.  [function <span class="apidocSignatureSpan">parker.</span>CssMediaQuery (raw)](#apidoc.element.parker.CssMediaQuery)
1.  [function <span class="apidocSignatureSpan">parker.</span>CssRule (raw)](#apidoc.element.parker.CssRule)
1.  [function <span class="apidocSignatureSpan">parker.</span>CssSelector (raw)](#apidoc.element.parker.CssSelector)
1.  [function <span class="apidocSignatureSpan">parker.</span>CssStylesheet (raw)](#apidoc.element.parker.CssStylesheet)
1.  object <span class="apidocSignatureSpan">parker.</span>CliController.prototype
1.  object <span class="apidocSignatureSpan">parker.</span>CliFormatter.prototype
1.  object <span class="apidocSignatureSpan">parker.</span>CssDeclaration.prototype
1.  object <span class="apidocSignatureSpan">parker.</span>CssMediaQuery.prototype
1.  object <span class="apidocSignatureSpan">parker.</span>CssRule.prototype
1.  object <span class="apidocSignatureSpan">parker.</span>CssSelector.prototype
1.  object <span class="apidocSignatureSpan">parker.</span>CssStylesheet.prototype
1.  object <span class="apidocSignatureSpan">parker.</span>Formatters
1.  object <span class="apidocSignatureSpan">parker.</span>IdentifiersPerSelector
1.  object <span class="apidocSignatureSpan">parker.</span>Info
1.  object <span class="apidocSignatureSpan">parker.</span>MediaQueries
1.  object <span class="apidocSignatureSpan">parker.</span>SelectorsPerRule
1.  object <span class="apidocSignatureSpan">parker.</span>SpecificityPerSelector
1.  object <span class="apidocSignatureSpan">parker.</span>TopSelectorSpecificity
1.  object <span class="apidocSignatureSpan">parker.</span>TopSelectorSpecificitySelector
1.  object <span class="apidocSignatureSpan">parker.</span>TotalDeclarations
1.  object <span class="apidocSignatureSpan">parker.</span>TotalIdSelectors
1.  object <span class="apidocSignatureSpan">parker.</span>TotalIdentifiers
1.  object <span class="apidocSignatureSpan">parker.</span>TotalImportantKeywords
1.  object <span class="apidocSignatureSpan">parker.</span>TotalMediaQueries
1.  object <span class="apidocSignatureSpan">parker.</span>TotalRules
1.  object <span class="apidocSignatureSpan">parker.</span>TotalSelectors
1.  object <span class="apidocSignatureSpan">parker.</span>TotalStylesheetSize
1.  object <span class="apidocSignatureSpan">parker.</span>TotalStylesheets
1.  object <span class="apidocSignatureSpan">parker.</span>TotalUniqueColours
1.  object <span class="apidocSignatureSpan">parker.</span>UniqueColours

#### [module parker.CliController](#apidoc.module.parker.CliController)
1.  [function <span class="apidocSignatureSpan">parker.</span>CliController ()](#apidoc.element.parker.CliController.CliController)
1.  [function <span class="apidocSignatureSpan">parker.CliController.</span>super_ ()](#apidoc.element.parker.CliController.super_)

#### [module parker.CliController.prototype](#apidoc.module.parker.CliController.prototype)
1.  [function <span class="apidocSignatureSpan">parker.CliController.prototype.</span>dispatch (argv)](#apidoc.element.parker.CliController.prototype.dispatch)

#### [module parker.CliFormatter](#apidoc.module.parker.CliFormatter)
1.  [function <span class="apidocSignatureSpan">parker.</span>CliFormatter ()](#apidoc.element.parker.CliFormatter.CliFormatter)

#### [module parker.CliFormatter.prototype](#apidoc.module.parker.CliFormatter.prototype)
1.  [function <span class="apidocSignatureSpan">parker.CliFormatter.prototype.</span>format (data, metrics)](#apidoc.element.parker.CliFormatter.prototype.format)

#### [module parker.CssDeclaration](#apidoc.module.parker.CssDeclaration)
1.  [function <span class="apidocSignatureSpan">parker.</span>CssDeclaration (raw)](#apidoc.element.parker.CssDeclaration.CssDeclaration)

#### [module parker.CssDeclaration.prototype](#apidoc.module.parker.CssDeclaration.prototype)
1.  [function <span class="apidocSignatureSpan">parker.CssDeclaration.prototype.</span>getProperty ()](#apidoc.element.parker.CssDeclaration.prototype.getProperty)
1.  [function <span class="apidocSignatureSpan">parker.CssDeclaration.prototype.</span>getValue ()](#apidoc.element.parker.CssDeclaration.prototype.getValue)

#### [module parker.CssMediaQuery](#apidoc.module.parker.CssMediaQuery)
1.  [function <span class="apidocSignatureSpan">parker.</span>CssMediaQuery (raw)](#apidoc.element.parker.CssMediaQuery.CssMediaQuery)

#### [module parker.CssMediaQuery.prototype](#apidoc.module.parker.CssMediaQuery.prototype)
1.  [function <span class="apidocSignatureSpan">parker.CssMediaQuery.prototype.</span>getQueries ()](#apidoc.element.parker.CssMediaQuery.prototype.getQueries)
1.  [function <span class="apidocSignatureSpan">parker.CssMediaQuery.prototype.</span>getRules ()](#apidoc.element.parker.CssMediaQuery.prototype.getRules)

#### [module parker.CssRule](#apidoc.module.parker.CssRule)
1.  [function <span class="apidocSignatureSpan">parker.</span>CssRule (raw)](#apidoc.element.parker.CssRule.CssRule)

#### [module parker.CssRule.prototype](#apidoc.module.parker.CssRule.prototype)
1.  [function <span class="apidocSignatureSpan">parker.CssRule.prototype.</span>getDeclarations ()](#apidoc.element.parker.CssRule.prototype.getDeclarations)
1.  [function <span class="apidocSignatureSpan">parker.CssRule.prototype.</span>getSelectors ()](#apidoc.element.parker.CssRule.prototype.getSelectors)

#### [module parker.CssSelector](#apidoc.module.parker.CssSelector)
1.  [function <span class="apidocSignatureSpan">parker.</span>CssSelector (raw)](#apidoc.element.parker.CssSelector.CssSelector)

#### [module parker.CssSelector.prototype](#apidoc.module.parker.CssSelector.prototype)
1.  [function <span class="apidocSignatureSpan">parker.CssSelector.prototype.</span>addIdentifier (identifier)](#apidoc.element.parker.CssSelector.prototype.addIdentifier)
1.  [function <span class="apidocSignatureSpan">parker.CssSelector.prototype.</span>getIdentifiers ()](#apidoc.element.parker.CssSelector.prototype.getIdentifiers)

#### [module parker.CssStylesheet](#apidoc.module.parker.CssStylesheet)
1.  [function <span class="apidocSignatureSpan">parker.</span>CssStylesheet (raw)](#apidoc.element.parker.CssStylesheet.CssStylesheet)

#### [module parker.CssStylesheet.prototype](#apidoc.module.parker.CssStylesheet.prototype)
1.  [function <span class="apidocSignatureSpan">parker.CssStylesheet.prototype.</span>getMalformedStatements ()](#apidoc.element.parker.CssStylesheet.prototype.getMalformedStatements)
1.  [function <span class="apidocSignatureSpan">parker.CssStylesheet.prototype.</span>getMediaQueries ()](#apidoc.element.parker.CssStylesheet.prototype.getMediaQueries)
1.  [function <span class="apidocSignatureSpan">parker.CssStylesheet.prototype.</span>getRules ()](#apidoc.element.parker.CssStylesheet.prototype.getRules)

#### [module parker.Formatters](#apidoc.module.parker.Formatters)
1.  [function <span class="apidocSignatureSpan">parker.Formatters.</span>csv (metrics, results)](#apidoc.element.parker.Formatters.csv)
1.  [function <span class="apidocSignatureSpan">parker.Formatters.</span>human (metrics, results)](#apidoc.element.parker.Formatters.human)
1.  [function <span class="apidocSignatureSpan">parker.Formatters.</span>json (metrics, results)](#apidoc.element.parker.Formatters.json)

#### [module parker.IdentifiersPerSelector](#apidoc.module.parker.IdentifiersPerSelector)
1.  [function <span class="apidocSignatureSpan">parker.IdentifiersPerSelector.</span>measure (selector)](#apidoc.element.parker.IdentifiersPerSelector.measure)
1.  string <span class="apidocSignatureSpan">parker.IdentifiersPerSelector.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.IdentifiersPerSelector.</span>format
1.  string <span class="apidocSignatureSpan">parker.IdentifiersPerSelector.</span>id
1.  string <span class="apidocSignatureSpan">parker.IdentifiersPerSelector.</span>name
1.  string <span class="apidocSignatureSpan">parker.IdentifiersPerSelector.</span>type

#### [module parker.Info](#apidoc.module.parker.Info)
1.  [function <span class="apidocSignatureSpan">parker.Info.</span>help ()](#apidoc.element.parker.Info.help)
1.  [function <span class="apidocSignatureSpan">parker.Info.</span>version ()](#apidoc.element.parker.Info.version)

#### [module parker.MediaQueries](#apidoc.module.parker.MediaQueries)
1.  [function <span class="apidocSignatureSpan">parker.MediaQueries.</span>filter (value, index, self)](#apidoc.element.parker.MediaQueries.filter)
1.  [function <span class="apidocSignatureSpan">parker.MediaQueries.</span>measure (query)](#apidoc.element.parker.MediaQueries.measure)
1.  string <span class="apidocSignatureSpan">parker.MediaQueries.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.MediaQueries.</span>format
1.  string <span class="apidocSignatureSpan">parker.MediaQueries.</span>id
1.  string <span class="apidocSignatureSpan">parker.MediaQueries.</span>name
1.  string <span class="apidocSignatureSpan">parker.MediaQueries.</span>type

#### [module parker.SelectorsPerRule](#apidoc.module.parker.SelectorsPerRule)
1.  [function <span class="apidocSignatureSpan">parker.SelectorsPerRule.</span>measure (rule)](#apidoc.element.parker.SelectorsPerRule.measure)
1.  string <span class="apidocSignatureSpan">parker.SelectorsPerRule.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.SelectorsPerRule.</span>format
1.  string <span class="apidocSignatureSpan">parker.SelectorsPerRule.</span>id
1.  string <span class="apidocSignatureSpan">parker.SelectorsPerRule.</span>name
1.  string <span class="apidocSignatureSpan">parker.SelectorsPerRule.</span>type

#### [module parker.SpecificityPerSelector](#apidoc.module.parker.SpecificityPerSelector)
1.  [function <span class="apidocSignatureSpan">parker.SpecificityPerSelector.</span>measure (rawSelector)](#apidoc.element.parker.SpecificityPerSelector.measure)
1.  string <span class="apidocSignatureSpan">parker.SpecificityPerSelector.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.SpecificityPerSelector.</span>format
1.  string <span class="apidocSignatureSpan">parker.SpecificityPerSelector.</span>id
1.  string <span class="apidocSignatureSpan">parker.SpecificityPerSelector.</span>name
1.  string <span class="apidocSignatureSpan">parker.SpecificityPerSelector.</span>type

#### [module parker.TopSelectorSpecificity](#apidoc.module.parker.TopSelectorSpecificity)
1.  [function <span class="apidocSignatureSpan">parker.TopSelectorSpecificity.</span>measure (rawSelector)](#apidoc.element.parker.TopSelectorSpecificity.measure)
1.  string <span class="apidocSignatureSpan">parker.TopSelectorSpecificity.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TopSelectorSpecificity.</span>format
1.  string <span class="apidocSignatureSpan">parker.TopSelectorSpecificity.</span>id
1.  string <span class="apidocSignatureSpan">parker.TopSelectorSpecificity.</span>name
1.  string <span class="apidocSignatureSpan">parker.TopSelectorSpecificity.</span>type

#### [module parker.TopSelectorSpecificitySelector](#apidoc.module.parker.TopSelectorSpecificitySelector)
1.  [function <span class="apidocSignatureSpan">parker.TopSelectorSpecificitySelector.</span>iterator (rawSelector)](#apidoc.element.parker.TopSelectorSpecificitySelector.iterator)
1.  [function <span class="apidocSignatureSpan">parker.TopSelectorSpecificitySelector.</span>measure (selector)](#apidoc.element.parker.TopSelectorSpecificitySelector.measure)
1.  string <span class="apidocSignatureSpan">parker.TopSelectorSpecificitySelector.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TopSelectorSpecificitySelector.</span>format
1.  string <span class="apidocSignatureSpan">parker.TopSelectorSpecificitySelector.</span>id
1.  string <span class="apidocSignatureSpan">parker.TopSelectorSpecificitySelector.</span>name
1.  string <span class="apidocSignatureSpan">parker.TopSelectorSpecificitySelector.</span>type

#### [module parker.TotalDeclarations](#apidoc.module.parker.TotalDeclarations)
1.  [function <span class="apidocSignatureSpan">parker.TotalDeclarations.</span>measure (declaration)](#apidoc.element.parker.TotalDeclarations.measure)
1.  string <span class="apidocSignatureSpan">parker.TotalDeclarations.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TotalDeclarations.</span>format
1.  string <span class="apidocSignatureSpan">parker.TotalDeclarations.</span>id
1.  string <span class="apidocSignatureSpan">parker.TotalDeclarations.</span>name
1.  string <span class="apidocSignatureSpan">parker.TotalDeclarations.</span>type

#### [module parker.TotalIdSelectors](#apidoc.module.parker.TotalIdSelectors)
1.  [function <span class="apidocSignatureSpan">parker.TotalIdSelectors.</span>measure (selector)](#apidoc.element.parker.TotalIdSelectors.measure)
1.  string <span class="apidocSignatureSpan">parker.TotalIdSelectors.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TotalIdSelectors.</span>format
1.  string <span class="apidocSignatureSpan">parker.TotalIdSelectors.</span>id
1.  string <span class="apidocSignatureSpan">parker.TotalIdSelectors.</span>name
1.  string <span class="apidocSignatureSpan">parker.TotalIdSelectors.</span>type

#### [module parker.TotalIdentifiers](#apidoc.module.parker.TotalIdentifiers)
1.  [function <span class="apidocSignatureSpan">parker.TotalIdentifiers.</span>measure (identifier)](#apidoc.element.parker.TotalIdentifiers.measure)
1.  string <span class="apidocSignatureSpan">parker.TotalIdentifiers.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TotalIdentifiers.</span>format
1.  string <span class="apidocSignatureSpan">parker.TotalIdentifiers.</span>id
1.  string <span class="apidocSignatureSpan">parker.TotalIdentifiers.</span>name
1.  string <span class="apidocSignatureSpan">parker.TotalIdentifiers.</span>type

#### [module parker.TotalImportantKeywords](#apidoc.module.parker.TotalImportantKeywords)
1.  [function <span class="apidocSignatureSpan">parker.TotalImportantKeywords.</span>measure (value)](#apidoc.element.parker.TotalImportantKeywords.measure)
1.  string <span class="apidocSignatureSpan">parker.TotalImportantKeywords.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TotalImportantKeywords.</span>format
1.  string <span class="apidocSignatureSpan">parker.TotalImportantKeywords.</span>id
1.  string <span class="apidocSignatureSpan">parker.TotalImportantKeywords.</span>name
1.  string <span class="apidocSignatureSpan">parker.TotalImportantKeywords.</span>type

#### [module parker.TotalMediaQueries](#apidoc.module.parker.TotalMediaQueries)
1.  [function <span class="apidocSignatureSpan">parker.TotalMediaQueries.</span>filter (value, index, self)](#apidoc.element.parker.TotalMediaQueries.filter)
1.  [function <span class="apidocSignatureSpan">parker.TotalMediaQueries.</span>measure (query)](#apidoc.element.parker.TotalMediaQueries.measure)
1.  string <span class="apidocSignatureSpan">parker.TotalMediaQueries.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TotalMediaQueries.</span>format
1.  string <span class="apidocSignatureSpan">parker.TotalMediaQueries.</span>id
1.  string <span class="apidocSignatureSpan">parker.TotalMediaQueries.</span>name
1.  string <span class="apidocSignatureSpan">parker.TotalMediaQueries.</span>type

#### [module parker.TotalRules](#apidoc.module.parker.TotalRules)
1.  [function <span class="apidocSignatureSpan">parker.TotalRules.</span>measure (rule)](#apidoc.element.parker.TotalRules.measure)
1.  string <span class="apidocSignatureSpan">parker.TotalRules.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TotalRules.</span>format
1.  string <span class="apidocSignatureSpan">parker.TotalRules.</span>id
1.  string <span class="apidocSignatureSpan">parker.TotalRules.</span>name
1.  string <span class="apidocSignatureSpan">parker.TotalRules.</span>type

#### [module parker.TotalSelectors](#apidoc.module.parker.TotalSelectors)
1.  [function <span class="apidocSignatureSpan">parker.TotalSelectors.</span>measure (selector)](#apidoc.element.parker.TotalSelectors.measure)
1.  string <span class="apidocSignatureSpan">parker.TotalSelectors.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TotalSelectors.</span>format
1.  string <span class="apidocSignatureSpan">parker.TotalSelectors.</span>id
1.  string <span class="apidocSignatureSpan">parker.TotalSelectors.</span>name
1.  string <span class="apidocSignatureSpan">parker.TotalSelectors.</span>type

#### [module parker.TotalStylesheetSize](#apidoc.module.parker.TotalStylesheetSize)
1.  [function <span class="apidocSignatureSpan">parker.TotalStylesheetSize.</span>measure (stylesheet)](#apidoc.element.parker.TotalStylesheetSize.measure)
1.  string <span class="apidocSignatureSpan">parker.TotalStylesheetSize.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TotalStylesheetSize.</span>format
1.  string <span class="apidocSignatureSpan">parker.TotalStylesheetSize.</span>id
1.  string <span class="apidocSignatureSpan">parker.TotalStylesheetSize.</span>name
1.  string <span class="apidocSignatureSpan">parker.TotalStylesheetSize.</span>type

#### [module parker.TotalStylesheets](#apidoc.module.parker.TotalStylesheets)
1.  [function <span class="apidocSignatureSpan">parker.TotalStylesheets.</span>measure (stylesheet)](#apidoc.element.parker.TotalStylesheets.measure)
1.  string <span class="apidocSignatureSpan">parker.TotalStylesheets.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TotalStylesheets.</span>format
1.  string <span class="apidocSignatureSpan">parker.TotalStylesheets.</span>id
1.  string <span class="apidocSignatureSpan">parker.TotalStylesheets.</span>name
1.  string <span class="apidocSignatureSpan">parker.TotalStylesheets.</span>type

#### [module parker.TotalUniqueColours](#apidoc.module.parker.TotalUniqueColours)
1.  [function <span class="apidocSignatureSpan">parker.TotalUniqueColours.</span>filter (value, index, self)](#apidoc.element.parker.TotalUniqueColours.filter)
1.  [function <span class="apidocSignatureSpan">parker.TotalUniqueColours.</span>measure (value)](#apidoc.element.parker.TotalUniqueColours.measure)
1.  string <span class="apidocSignatureSpan">parker.TotalUniqueColours.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.TotalUniqueColours.</span>format
1.  string <span class="apidocSignatureSpan">parker.TotalUniqueColours.</span>id
1.  string <span class="apidocSignatureSpan">parker.TotalUniqueColours.</span>name
1.  string <span class="apidocSignatureSpan">parker.TotalUniqueColours.</span>type

#### [module parker.UniqueColours](#apidoc.module.parker.UniqueColours)
1.  [function <span class="apidocSignatureSpan">parker.UniqueColours.</span>filter (value, index, self)](#apidoc.element.parker.UniqueColours.filter)
1.  [function <span class="apidocSignatureSpan">parker.UniqueColours.</span>measure (value)](#apidoc.element.parker.UniqueColours.measure)
1.  string <span class="apidocSignatureSpan">parker.UniqueColours.</span>aggregate
1.  string <span class="apidocSignatureSpan">parker.UniqueColours.</span>format
1.  string <span class="apidocSignatureSpan">parker.UniqueColours.</span>id
1.  string <span class="apidocSignatureSpan">parker.UniqueColours.</span>name
1.  string <span class="apidocSignatureSpan">parker.UniqueColours.</span>type



# <a name="apidoc.module.parker"></a>[module parker](#apidoc.module.parker)

#### <a name="apidoc.element.parker.CliController"></a>[function <span class="apidocSignatureSpan">parker.</span>CliController ()](#apidoc.element.parker.CliController)
- description and source-code
```javascript
function CliController() {
    events.EventEmitter.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CliFormatter"></a>[function <span class="apidocSignatureSpan">parker.</span>CliFormatter ()](#apidoc.element.parker.CliFormatter)
- description and source-code
```javascript
function CliFormatter() {

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CssDeclaration"></a>[function <span class="apidocSignatureSpan">parker.</span>CssDeclaration (raw)](#apidoc.element.parker.CssDeclaration)
- description and source-code
```javascript
function CssDeclaration(raw) {

    this.raw = raw;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CssMediaQuery"></a>[function <span class="apidocSignatureSpan">parker.</span>CssMediaQuery (raw)](#apidoc.element.parker.CssMediaQuery)
- description and source-code
```javascript
function CssMediaQuery(raw) {
	this.raw = raw;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CssRule"></a>[function <span class="apidocSignatureSpan">parker.</span>CssRule (raw)](#apidoc.element.parker.CssRule)
- description and source-code
```javascript
function CssRule(raw) {
    this.raw = raw;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CssSelector"></a>[function <span class="apidocSignatureSpan">parker.</span>CssSelector (raw)](#apidoc.element.parker.CssSelector)
- description and source-code
```javascript
function CssSelector(raw) {
    this.raw = raw;
    this.identifiers = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CssStylesheet"></a>[function <span class="apidocSignatureSpan">parker.</span>CssStylesheet (raw)](#apidoc.element.parker.CssStylesheet)
- description and source-code
```javascript
function CssStylesheet(raw) {
    this.raw = raw;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CliController"></a>[module parker.CliController](#apidoc.module.parker.CliController)

#### <a name="apidoc.element.parker.CliController.CliController"></a>[function <span class="apidocSignatureSpan">parker.</span>CliController ()](#apidoc.element.parker.CliController.CliController)
- description and source-code
```javascript
function CliController() {
    events.EventEmitter.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CliController.super_"></a>[function <span class="apidocSignatureSpan">parker.CliController.</span>super_ ()](#apidoc.element.parker.CliController.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CliController.prototype"></a>[module parker.CliController.prototype](#apidoc.module.parker.CliController.prototype)

#### <a name="apidoc.element.parker.CliController.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">parker.CliController.prototype.</span>dispatch (argv)](#apidoc.element.parker.CliController.prototype.dispatch)
- description and source-code
```javascript
dispatch = function (argv) {
    if (argv.v || argv.version) {
        this.emit('showVersion');
    }
    if (argv.h || argv.help) {
        this.emit('showHelp');
    }
    if (argv.f || argv.format) {
        var format = argv.f || argv.format;
        this.emit('setFormat', format);
    }
    if (argv.n || argv.numeric) {
        this.emit('showNumericOnly');
    }
    if (argv._ && argv._.length) {
        this.emit('runPaths', argv._);
    }
    else if (argv.s || argv.stdin) {
        this.emit('runStdin');
    }
    else {
        // No data supplied - show help
        this.emit('showHelp');
    }
}
```
- example usage
```shell
...
};

if (module.parent) {
    module.exports = Parker;
} else {
    var parker = new Parker(metrics),
    formatter = formatters['human'];
    cliController.dispatch(argv);
}
...
```



# <a name="apidoc.module.parker.CliFormatter"></a>[module parker.CliFormatter](#apidoc.module.parker.CliFormatter)

#### <a name="apidoc.element.parker.CliFormatter.CliFormatter"></a>[function <span class="apidocSignatureSpan">parker.</span>CliFormatter ()](#apidoc.element.parker.CliFormatter.CliFormatter)
- description and source-code
```javascript
function CliFormatter() {

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CliFormatter.prototype"></a>[module parker.CliFormatter.prototype](#apidoc.module.parker.CliFormatter.prototype)

#### <a name="apidoc.element.parker.CliFormatter.prototype.format"></a>[function <span class="apidocSignatureSpan">parker.CliFormatter.prototype.</span>format (data, metrics)](#apidoc.element.parker.CliFormatter.prototype.format)
- description and source-code
```javascript
format = function (data, metrics) {
	var output = '';
    _.each(metrics, function(metric) {
        output += metric.name + ": " + data[metric.id];
        output += "\n";
    });

	return output;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CssDeclaration"></a>[module parker.CssDeclaration](#apidoc.module.parker.CssDeclaration)

#### <a name="apidoc.element.parker.CssDeclaration.CssDeclaration"></a>[function <span class="apidocSignatureSpan">parker.</span>CssDeclaration (raw)](#apidoc.element.parker.CssDeclaration.CssDeclaration)
- description and source-code
```javascript
function CssDeclaration(raw) {

    this.raw = raw;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CssDeclaration.prototype"></a>[module parker.CssDeclaration.prototype](#apidoc.module.parker.CssDeclaration.prototype)

#### <a name="apidoc.element.parker.CssDeclaration.prototype.getProperty"></a>[function <span class="apidocSignatureSpan">parker.CssDeclaration.prototype.</span>getProperty ()](#apidoc.element.parker.CssDeclaration.prototype.getProperty)
- description and source-code
```javascript
getProperty = function () {
    if (this.raw.indexOf(':') === -1) {
        return '';
    }

    return this.raw.split(':')[0].trim();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CssDeclaration.prototype.getValue"></a>[function <span class="apidocSignatureSpan">parker.CssDeclaration.prototype.</span>getValue ()](#apidoc.element.parker.CssDeclaration.prototype.getValue)
- description and source-code
```javascript
getValue = function () {
    if (this.raw.indexOf(':') === -1) {
        return '';
    }

    return this.raw.split(':')[1].trim();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CssMediaQuery"></a>[module parker.CssMediaQuery](#apidoc.module.parker.CssMediaQuery)

#### <a name="apidoc.element.parker.CssMediaQuery.CssMediaQuery"></a>[function <span class="apidocSignatureSpan">parker.</span>CssMediaQuery (raw)](#apidoc.element.parker.CssMediaQuery.CssMediaQuery)
- description and source-code
```javascript
function CssMediaQuery(raw) {
	this.raw = raw;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CssMediaQuery.prototype"></a>[module parker.CssMediaQuery.prototype](#apidoc.module.parker.CssMediaQuery.prototype)

#### <a name="apidoc.element.parker.CssMediaQuery.prototype.getQueries"></a>[function <span class="apidocSignatureSpan">parker.CssMediaQuery.prototype.</span>getQueries ()](#apidoc.element.parker.CssMediaQuery.prototype.getQueries)
- description and source-code
```javascript
getQueries = function () {
	var pattern = /@media\w*(.+?)\s?{/,
		queries = pattern.exec(this.raw)[1];

	return queries.split(/ or |,/g).map(trimQuery);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CssMediaQuery.prototype.getRules"></a>[function <span class="apidocSignatureSpan">parker.CssMediaQuery.prototype.</span>getRules ()](#apidoc.element.parker.CssMediaQuery.prototype.getRules)
- description and source-code
```javascript
getRules = function () {
    var rules = [],
        depth = 0,
        rule = '';

    for (var index = 0; index < this.raw.length; index++) {
    	if (depth > 0) {
	        rule += this.raw.charAt(index);
	    }
        if (this.raw.charAt(index) === '{') {
            depth ++;
        }
        else if (this.raw.charAt(index) == '}') {
            depth --;
        }

        if (depth === 1 && this.raw.charAt(index) == '}') {
            rules.push(rule.trim());
            rule = '';
        }
    }
    return rules;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CssRule"></a>[module parker.CssRule](#apidoc.module.parker.CssRule)

#### <a name="apidoc.element.parker.CssRule.CssRule"></a>[function <span class="apidocSignatureSpan">parker.</span>CssRule (raw)](#apidoc.element.parker.CssRule.CssRule)
- description and source-code
```javascript
function CssRule(raw) {
    this.raw = raw;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CssRule.prototype"></a>[module parker.CssRule.prototype](#apidoc.module.parker.CssRule.prototype)

#### <a name="apidoc.element.parker.CssRule.prototype.getDeclarations"></a>[function <span class="apidocSignatureSpan">parker.CssRule.prototype.</span>getDeclarations ()](#apidoc.element.parker.CssRule.prototype.getDeclarations)
- description and source-code
```javascript
getDeclarations = function () {
    return getDeclarations(getDeclarationBlock(this.raw));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CssRule.prototype.getSelectors"></a>[function <span class="apidocSignatureSpan">parker.CssRule.prototype.</span>getSelectors ()](#apidoc.element.parker.CssRule.prototype.getSelectors)
- description and source-code
```javascript
getSelectors = function () {
    return getSelectors(getSelectorBlock(this.raw));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CssSelector"></a>[module parker.CssSelector](#apidoc.module.parker.CssSelector)

#### <a name="apidoc.element.parker.CssSelector.CssSelector"></a>[function <span class="apidocSignatureSpan">parker.</span>CssSelector (raw)](#apidoc.element.parker.CssSelector.CssSelector)
- description and source-code
```javascript
function CssSelector(raw) {
    this.raw = raw;
    this.identifiers = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CssSelector.prototype"></a>[module parker.CssSelector.prototype](#apidoc.module.parker.CssSelector.prototype)

#### <a name="apidoc.element.parker.CssSelector.prototype.addIdentifier"></a>[function <span class="apidocSignatureSpan">parker.CssSelector.prototype.</span>addIdentifier (identifier)](#apidoc.element.parker.CssSelector.prototype.addIdentifier)
- description and source-code
```javascript
addIdentifier = function (identifier) {
    this.identifiers.push(identifier);
}
```
- example usage
```shell
...
parenDepth = 0;

    _.each(this.raw, function (character, index) {
var insideBrackets = bracketDepth || parenDepth,
    isSecondColon = character == ':' && this.raw[index - 1] == ':';

if (!insideBrackets && isDelimiter(character) && !isSecondColon) {
    this.addIdentifier(identifier);
    identifier = '';
}

switch(character) {
    case '(': parenDepth++; break;
    case ')': parenDepth--; break;
    case '[': bracketDepth++; break;
...
```

#### <a name="apidoc.element.parker.CssSelector.prototype.getIdentifiers"></a>[function <span class="apidocSignatureSpan">parker.CssSelector.prototype.</span>getIdentifiers ()](#apidoc.element.parker.CssSelector.prototype.getIdentifiers)
- description and source-code
```javascript
getIdentifiers = function () {
    var identifier = '',
        bracketDepth = 0,
        parenDepth = 0;

    _.each(this.raw, function (character, index) {
        var insideBrackets = bracketDepth || parenDepth,
            isSecondColon = character == ':' && this.raw[index - 1] == ':';

        if (!insideBrackets && isDelimiter(character) && !isSecondColon) {
            this.addIdentifier(identifier);
            identifier = '';
        }

        switch(character) {
            case '(': parenDepth++; break;
            case ')': parenDepth--; break;
            case '[': bracketDepth++; break;
            case ']': bracketDepth--; break;
        }

        if (!_.contains([' ', '>'], character)) {
            identifier += character;
        }
    }, this);

    this.addIdentifier(identifier);
    return _.without(this.identifiers, ' ', '', '[]');
}
```
- example usage
```shell
...
    type: 'selector',
    aggregate: 'mean',
    format: 'number',
    measure: function (rawSelector) {
var totalSpecificity = 0,
    selector = new CssSelector(rawSelector);

_.each(selector.getIdentifiers(), function (identifier) {
    var idIdentifiers = countIdIdentifiers(identifier),
        classIdentifiers = countClassIdentifiers(identifier),
        attributeIdentifiers = countAttributeIdentifiers(identifier),
        pseudoClassIdentifiers = countPseudoClassIdentifiers(identifier),
        typeIdentifiers = countTypeIdentifiers(identifier),
        pseudoElementIdentifiers = countPseudoElementIdentifiers(identifier);
...
```



# <a name="apidoc.module.parker.CssStylesheet"></a>[module parker.CssStylesheet](#apidoc.module.parker.CssStylesheet)

#### <a name="apidoc.element.parker.CssStylesheet.CssStylesheet"></a>[function <span class="apidocSignatureSpan">parker.</span>CssStylesheet (raw)](#apidoc.element.parker.CssStylesheet.CssStylesheet)
- description and source-code
```javascript
function CssStylesheet(raw) {
    this.raw = raw;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.CssStylesheet.prototype"></a>[module parker.CssStylesheet.prototype](#apidoc.module.parker.CssStylesheet.prototype)

#### <a name="apidoc.element.parker.CssStylesheet.prototype.getMalformedStatements"></a>[function <span class="apidocSignatureSpan">parker.CssStylesheet.prototype.</span>getMalformedStatements ()](#apidoc.element.parker.CssStylesheet.prototype.getMalformedStatements)
- description and source-code
```javascript
getMalformedStatements = function () {
    this.children = this.children || getChildren(this.raw);

    return this.children.filter(function (child) {
        return isMalformedStatement(child);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CssStylesheet.prototype.getMediaQueries"></a>[function <span class="apidocSignatureSpan">parker.CssStylesheet.prototype.</span>getMediaQueries ()](#apidoc.element.parker.CssStylesheet.prototype.getMediaQueries)
- description and source-code
```javascript
getMediaQueries = function () {
    this.children = this.children || getChildren(this.raw);
    return this.children.filter(function (child) {
        return isMediaQuery(child);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.CssStylesheet.prototype.getRules"></a>[function <span class="apidocSignatureSpan">parker.CssStylesheet.prototype.</span>getRules ()](#apidoc.element.parker.CssStylesheet.prototype.getRules)
- description and source-code
```javascript
getRules = function () {
    this.children = this.children || getChildren(this.raw);

    return this.children.filter(function (child) {
        return isRule(child);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.Formatters"></a>[module parker.Formatters](#apidoc.module.parker.Formatters)

#### <a name="apidoc.element.parker.Formatters.csv"></a>[function <span class="apidocSignatureSpan">parker.Formatters.</span>csv (metrics, results)](#apidoc.element.parker.Formatters.csv)
- description and source-code
```javascript
csv = function (metrics, results) {
    var lineItems = [];
    _.each(metrics, function (metric) {
        lineItems.push('"' + results[metric.id] + '"');
    });

    return lineItems.join(',');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.Formatters.human"></a>[function <span class="apidocSignatureSpan">parker.Formatters.</span>human (metrics, results)](#apidoc.element.parker.Formatters.human)
- description and source-code
```javascript
human = function (metrics, results) {
    var logo = clc.red('PA') + clc.yellow('RK') + clc.green('ER') + '-JS' + "\n";
    return logo + _.reduce(metrics, function (str, metric) {
        return str + metric.name + ': ' + results[metric.id] + '\n';
    }, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.Formatters.json"></a>[function <span class="apidocSignatureSpan">parker.Formatters.</span>json (metrics, results)](#apidoc.element.parker.Formatters.json)
- description and source-code
```javascript
json = function (metrics, results) {
    var ids = _.map(metrics, function (metric) {
        return metric.id;
    });
    var obj = _.reduce(ids, function (obj, id) {
        obj[id] = results[id];
        return obj;
    }, {});
    return JSON.stringify(obj, null, 4);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.IdentifiersPerSelector"></a>[module parker.IdentifiersPerSelector](#apidoc.module.parker.IdentifiersPerSelector)

#### <a name="apidoc.element.parker.IdentifiersPerSelector.measure"></a>[function <span class="apidocSignatureSpan">parker.IdentifiersPerSelector.</span>measure (selector)](#apidoc.element.parker.IdentifiersPerSelector.measure)
- description and source-code
```javascript
measure = function (selector) {
    var identifiers = getIdentifiers(selector);

    if (identifiers.length === 1 && identifiers[0] === '') {
        return 0;
    }

    return identifiers.length;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.Info"></a>[module parker.Info](#apidoc.module.parker.Info)

#### <a name="apidoc.element.parker.Info.help"></a>[function <span class="apidocSignatureSpan">parker.Info.</span>help ()](#apidoc.element.parker.Info.help)
- description and source-code
```javascript
help = function () {
    module.exports.version();

    [
        pkg.description,
        '',
        'Usage:',
        'parker [arguments] [file...] Run Parker on specified files',
        '',
        'Example Local Usage:',
        'parker styles.css',
        '',
        'Example Stdin Usage:',
        'curl http://www.katiefenn.co.uk/css/shuttle.css -s | parker -s',
        '',
        'Arguments:',
        '',
        '-f                  Set output format (see list of formats)',
        '-h                  Shows help',
        '-n                  Show numeric results only',
        '-s                  Input CSS using stdin',
        '-v                  Show version number of Parker',
        '',
        'Formats Usage:',
        'parker -f "human"',
        '',
        'Formats List:',
        'human               Human-readable, newline separated format (default)',
        'json                JSON',
        'csv                 CSV',
        '',
        'For more information, see ' + pkg.homepage
    ].forEach(function(str) { console.log(str); });
}
```
- example usage
```shell
...

cliController.on('showVersion', function () {
info.version();
process.exit();
});

cliController.on('showHelp', function () {
info.help();
process.exit();
});

cliController.on('setFormat', function (format) {
formatter = formatters[format];

if (!formatter) {
...
```

#### <a name="apidoc.element.parker.Info.version"></a>[function <span class="apidocSignatureSpan">parker.Info.</span>version ()](#apidoc.element.parker.Info.version)
- description and source-code
```javascript
version = function () {
    console.log(pkg.name + ' v' + pkg.version);
}
```
- example usage
```shell
...

    process.stdin.on('end', function() {
        runReport(stdinData, metrics);
    });
});

cliController.on('showVersion', function () {
    info.version();
    process.exit();
});

cliController.on('showHelp', function () {
    info.help();
    process.exit();
});
...
```



# <a name="apidoc.module.parker.MediaQueries"></a>[module parker.MediaQueries](#apidoc.module.parker.MediaQueries)

#### <a name="apidoc.element.parker.MediaQueries.filter"></a>[function <span class="apidocSignatureSpan">parker.MediaQueries.</span>filter (value, index, self)](#apidoc.element.parker.MediaQueries.filter)
- description and source-code
```javascript
filter = function (value, index, self) {
    return self.indexOf(value) === index;
}
```
- example usage
```shell
...
    console.error('Unknown output format: %s', argv.format);
    console.error('  available: ' + Object.keys(formatters).join(' '));
    process.exit(1);
}
});

cliController.on('showNumericOnly', function () {
metrics = _.filter(metrics, function (metric) {
    return metric.format == 'number';
});
});

var readDirectory = function (directoryPath, onFileLoad, onAllLoad) {
fs.readdir(directoryPath, function (err, files) {
    async.each(files, function (file, fileDone) {
...
```

#### <a name="apidoc.element.parker.MediaQueries.measure"></a>[function <span class="apidocSignatureSpan">parker.MediaQueries.</span>measure (query)](#apidoc.element.parker.MediaQueries.measure)
- description and source-code
```javascript
measure = function (query) {
    return query;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.SelectorsPerRule"></a>[module parker.SelectorsPerRule](#apidoc.module.parker.SelectorsPerRule)

#### <a name="apidoc.element.parker.SelectorsPerRule.measure"></a>[function <span class="apidocSignatureSpan">parker.SelectorsPerRule.</span>measure (rule)](#apidoc.element.parker.SelectorsPerRule.measure)
- description and source-code
```javascript
measure = function (rule) {
    return getSelectors(getSelectorBlock(rule)).length;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.SpecificityPerSelector"></a>[module parker.SpecificityPerSelector](#apidoc.module.parker.SpecificityPerSelector)

#### <a name="apidoc.element.parker.SpecificityPerSelector.measure"></a>[function <span class="apidocSignatureSpan">parker.SpecificityPerSelector.</span>measure (rawSelector)](#apidoc.element.parker.SpecificityPerSelector.measure)
- description and source-code
```javascript
measure = function (rawSelector) {
    var totalSpecificity = 0,
        selector = new CssSelector(rawSelector);

    _.each(selector.getIdentifiers(), function (identifier) {
        var idIdentifiers = countIdIdentifiers(identifier),
            classIdentifiers = countClassIdentifiers(identifier),
            attributeIdentifiers = countAttributeIdentifiers(identifier),
            pseudoClassIdentifiers = countPseudoClassIdentifiers(identifier),
            typeIdentifiers = countTypeIdentifiers(identifier),
            pseudoElementIdentifiers = countPseudoElementIdentifiers(identifier);

        totalSpecificity += Number(
            String(idIdentifiers) +
            String(classIdentifiers + attributeIdentifiers + pseudoClassIdentifiers) +
            String(typeIdentifiers + pseudoElementIdentifiers));
    });

    return totalSpecificity;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TopSelectorSpecificity"></a>[module parker.TopSelectorSpecificity](#apidoc.module.parker.TopSelectorSpecificity)

#### <a name="apidoc.element.parker.TopSelectorSpecificity.measure"></a>[function <span class="apidocSignatureSpan">parker.TopSelectorSpecificity.</span>measure (rawSelector)](#apidoc.element.parker.TopSelectorSpecificity.measure)
- description and source-code
```javascript
measure = function (rawSelector) {
    var selector = new CssSelector(rawSelector),
        identifiers = selector.getIdentifiers(),
        specificity = 0;

    _.each(identifiers, function (identifier) {
        identifier = stripNotIdentifier(identifier);

        var idIdentifiers = countIdIdentifiers(identifier),
            classIdentifiers = countClassIdentifiers(identifier),
            attributeIdentifiers = countAttributeIdentifiers(identifier),
            pseudoClassIdentifiers = countPseudoClassIdentifiers(identifier),
            typeIdentifiers = countTypeIdentifiers(identifier),
            pseudoElementIdentifiers = countPseudoElementIdentifiers(identifier);

        specificity += getSpecificity(idIdentifiers, classIdentifiers, attributeIdentifiers, pseudoClassIdentifiers, typeIdentifiers
, pseudoElementIdentifiers);

    }, this);

    return specificity;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TopSelectorSpecificitySelector"></a>[module parker.TopSelectorSpecificitySelector](#apidoc.module.parker.TopSelectorSpecificitySelector)

#### <a name="apidoc.element.parker.TopSelectorSpecificitySelector.iterator"></a>[function <span class="apidocSignatureSpan">parker.TopSelectorSpecificitySelector.</span>iterator (rawSelector)](#apidoc.element.parker.TopSelectorSpecificitySelector.iterator)
- description and source-code
```javascript
iterator = function (rawSelector) {
    var selector = new CssSelector(rawSelector),
        identifiers = selector.getIdentifiers(),
        specificity = 0;

    _.each(identifiers, function (identifier) {
        var idIdentifiers = countIdIdentifiers(identifier),
            classIdentifiers = countClassIdentifiers(identifier),
            attributeIdentifiers = countAttributeIdentifiers(identifier),
            pseudoClassIdentifiers = countPseudoClassIdentifiers(identifier),
            typeIdentifiers = countTypeIdentifiers(identifier),
            pseudoElementIdentifiers = countPseudoElementIdentifiers(identifier);

        specificity += getSpecificity(idIdentifiers, classIdentifiers, attributeIdentifiers, pseudoClassIdentifiers, typeIdentifiers
, pseudoElementIdentifiers);

    }, this);

    return specificity;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parker.TopSelectorSpecificitySelector.measure"></a>[function <span class="apidocSignatureSpan">parker.TopSelectorSpecificitySelector.</span>measure (selector)](#apidoc.element.parker.TopSelectorSpecificitySelector.measure)
- description and source-code
```javascript
measure = function (selector) {
    return selector;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TotalDeclarations"></a>[module parker.TotalDeclarations](#apidoc.module.parker.TotalDeclarations)

#### <a name="apidoc.element.parker.TotalDeclarations.measure"></a>[function <span class="apidocSignatureSpan">parker.TotalDeclarations.</span>measure (declaration)](#apidoc.element.parker.TotalDeclarations.measure)
- description and source-code
```javascript
measure = function (declaration) {
    return 1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TotalIdSelectors"></a>[module parker.TotalIdSelectors](#apidoc.module.parker.TotalIdSelectors)

#### <a name="apidoc.element.parker.TotalIdSelectors.measure"></a>[function <span class="apidocSignatureSpan">parker.TotalIdSelectors.</span>measure (selector)](#apidoc.element.parker.TotalIdSelectors.measure)
- description and source-code
```javascript
measure = function (selector) {
		var ids = 0;
		var inBrackets = false;

		_.forOwn(selector, function (char) {
			if (char === '[') {
				inBrackets = true;
			} else if (char === ']') {
				inBrackets = false;
			} else if (char === '#' && !inBrackets) {
				ids++;
			}
		});

		return ids;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TotalIdentifiers"></a>[module parker.TotalIdentifiers](#apidoc.module.parker.TotalIdentifiers)

#### <a name="apidoc.element.parker.TotalIdentifiers.measure"></a>[function <span class="apidocSignatureSpan">parker.TotalIdentifiers.</span>measure (identifier)](#apidoc.element.parker.TotalIdentifiers.measure)
- description and source-code
```javascript
measure = function (identifier) {
    return 1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TotalImportantKeywords"></a>[module parker.TotalImportantKeywords](#apidoc.module.parker.TotalImportantKeywords)

#### <a name="apidoc.element.parker.TotalImportantKeywords.measure"></a>[function <span class="apidocSignatureSpan">parker.TotalImportantKeywords.</span>measure (value)](#apidoc.element.parker.TotalImportantKeywords.measure)
- description and source-code
```javascript
measure = function (value) {
    if (value.match(/!important/g))
        return 1;
    return 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TotalMediaQueries"></a>[module parker.TotalMediaQueries](#apidoc.module.parker.TotalMediaQueries)

#### <a name="apidoc.element.parker.TotalMediaQueries.filter"></a>[function <span class="apidocSignatureSpan">parker.TotalMediaQueries.</span>filter (value, index, self)](#apidoc.element.parker.TotalMediaQueries.filter)
- description and source-code
```javascript
filter = function (value, index, self) {
    return self.indexOf(value) === index;
}
```
- example usage
```shell
...
    console.error('Unknown output format: %s', argv.format);
    console.error('  available: ' + Object.keys(formatters).join(' '));
    process.exit(1);
}
});

cliController.on('showNumericOnly', function () {
metrics = _.filter(metrics, function (metric) {
    return metric.format == 'number';
});
});

var readDirectory = function (directoryPath, onFileLoad, onAllLoad) {
fs.readdir(directoryPath, function (err, files) {
    async.each(files, function (file, fileDone) {
...
```

#### <a name="apidoc.element.parker.TotalMediaQueries.measure"></a>[function <span class="apidocSignatureSpan">parker.TotalMediaQueries.</span>measure (query)](#apidoc.element.parker.TotalMediaQueries.measure)
- description and source-code
```javascript
measure = function (query) {
    return query;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TotalRules"></a>[module parker.TotalRules](#apidoc.module.parker.TotalRules)

#### <a name="apidoc.element.parker.TotalRules.measure"></a>[function <span class="apidocSignatureSpan">parker.TotalRules.</span>measure (rule)](#apidoc.element.parker.TotalRules.measure)
- description and source-code
```javascript
measure = function (rule) {
    return 1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TotalSelectors"></a>[module parker.TotalSelectors](#apidoc.module.parker.TotalSelectors)

#### <a name="apidoc.element.parker.TotalSelectors.measure"></a>[function <span class="apidocSignatureSpan">parker.TotalSelectors.</span>measure (selector)](#apidoc.element.parker.TotalSelectors.measure)
- description and source-code
```javascript
measure = function (selector) {
    return 1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TotalStylesheetSize"></a>[module parker.TotalStylesheetSize](#apidoc.module.parker.TotalStylesheetSize)

#### <a name="apidoc.element.parker.TotalStylesheetSize.measure"></a>[function <span class="apidocSignatureSpan">parker.TotalStylesheetSize.</span>measure (stylesheet)](#apidoc.element.parker.TotalStylesheetSize.measure)
- description and source-code
```javascript
measure = function (stylesheet) {
    return byteCount(stylesheet);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TotalStylesheets"></a>[module parker.TotalStylesheets](#apidoc.module.parker.TotalStylesheets)

#### <a name="apidoc.element.parker.TotalStylesheets.measure"></a>[function <span class="apidocSignatureSpan">parker.TotalStylesheets.</span>measure (stylesheet)](#apidoc.element.parker.TotalStylesheets.measure)
- description and source-code
```javascript
measure = function (stylesheet) {
    return 1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.TotalUniqueColours"></a>[module parker.TotalUniqueColours](#apidoc.module.parker.TotalUniqueColours)

#### <a name="apidoc.element.parker.TotalUniqueColours.filter"></a>[function <span class="apidocSignatureSpan">parker.TotalUniqueColours.</span>filter (value, index, self)](#apidoc.element.parker.TotalUniqueColours.filter)
- description and source-code
```javascript
filter = function (value, index, self) {
    return self.indexOf(value) === index;
}
```
- example usage
```shell
...
    console.error('Unknown output format: %s', argv.format);
    console.error('  available: ' + Object.keys(formatters).join(' '));
    process.exit(1);
}
});

cliController.on('showNumericOnly', function () {
metrics = _.filter(metrics, function (metric) {
    return metric.format == 'number';
});
});

var readDirectory = function (directoryPath, onFileLoad, onAllLoad) {
fs.readdir(directoryPath, function (err, files) {
    async.each(files, function (file, fileDone) {
...
```

#### <a name="apidoc.element.parker.TotalUniqueColours.measure"></a>[function <span class="apidocSignatureSpan">parker.TotalUniqueColours.</span>measure (value)](#apidoc.element.parker.TotalUniqueColours.measure)
- description and source-code
```javascript
measure = function (value) {
    return getColourHexes(value).map(function (colourHex) {
        return getLongHashForm(colourHex).toUpperCase();
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parker.UniqueColours"></a>[module parker.UniqueColours](#apidoc.module.parker.UniqueColours)

#### <a name="apidoc.element.parker.UniqueColours.filter"></a>[function <span class="apidocSignatureSpan">parker.UniqueColours.</span>filter (value, index, self)](#apidoc.element.parker.UniqueColours.filter)
- description and source-code
```javascript
filter = function (value, index, self) {
    return self.indexOf(value) === index;
}
```
- example usage
```shell
...
    console.error('Unknown output format: %s', argv.format);
    console.error('  available: ' + Object.keys(formatters).join(' '));
    process.exit(1);
}
});

cliController.on('showNumericOnly', function () {
metrics = _.filter(metrics, function (metric) {
    return metric.format == 'number';
});
});

var readDirectory = function (directoryPath, onFileLoad, onAllLoad) {
fs.readdir(directoryPath, function (err, files) {
    async.each(files, function (file, fileDone) {
...
```

#### <a name="apidoc.element.parker.UniqueColours.measure"></a>[function <span class="apidocSignatureSpan">parker.UniqueColours.</span>measure (value)](#apidoc.element.parker.UniqueColours.measure)
- description and source-code
```javascript
measure = function (value) {
    return getColourHexes(value).map(function (colourHex) {
        return getLongHashForm(colourHex).toUpperCase();
    });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
