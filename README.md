# npmtest-swagger-parser

#### basic test coverage for  [swagger-parser (v3.4.1)](https://bigstickcarpet.github.io/swagger-parser)  [![npm package](https://img.shields.io/npm/v/npmtest-swagger-parser.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-swagger-parser) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-swagger-parser.svg)](https://travis-ci.org/npmtest/node-npmtest-swagger-parser)

#### Swagger 2.0 parser and validator for Node and browsers

[![NPM](https://nodei.co/npm/swagger-parser.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/swagger-parser)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-swagger-parser/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-swagger-parser/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-swagger-parser/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-swagger-parser/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-swagger-parser/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-swagger-parser/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-swagger-parser/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-swagger-parser/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-swagger-parser/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-swagger-parser/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-swagger-parser/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-swagger-parser/build/test-report.html](https://npmtest.github.io/node-npmtest-swagger-parser/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-swagger-parser/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-swagger-parser/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-swagger-parser/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-swagger-parser/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-swagger-parser/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-swagger-parser/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-swagger-parser/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-swagger-parser/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "swagger-parser",
    "version": "3.4.1",
    "description": "Swagger 2.0 parser and validator for Node and browsers",
    "keywords": [
        "swagger",
        "json",
        "yaml",
        "parse",
        "parser",
        "validate",
        "validator",
        "validation",
        "spec",
        "specification",
        "schema",
        "reference",
        "dereference"
    ],
    "author": {
        "name": "James Messinger",
        "url": "http://jamesmessinger.com"
    },
    "license": "MIT",
    "homepage": "https://bigstickcarpet.github.io/swagger-parser",
    "main": "lib/index.js",
    "scripts": {
        "lint": "eslint lib && jscs lib --verbose",
        "build": "npm run lint && npm run browserify && npm run build-www",
        "browserify": "simplifyify lib/index.js --outfile dist/swagger-parser.js --standalone SwaggerParser --bundle --debug --minify",
        "watch": "npm run browserify -- --watch & npm run browserify-www -- --watch",
        "mocha": "mocha --bail --async-only --recursive tests/fixtures tests/specs",
        "istanbul": "istanbul cover _mocha --dir coverage/node -- --bail --recursive tests/fixtures tests/specs",
        "karma": "karma start --single-run",
        "test": "npm run browserify -- --test && npm run istanbul && npm run karma",
        "upgrade": "ncu --upgradeAll && npm update && bower update",
        "bump": "bump --prompt --grep lib/index.js dist/* --tag --push --all",
        "release": "npm run upgrade && npm run build-www && npm test && npm run bump && npm publish",
        "build-www": "npm run sass && npm run browserify-www",
        "browserify-www": "simplifyify www/js/index.js --outfile www/js/bundle.js --bundle --debug --minify",
        "sass": "node-sass --source-map true --output-style compressed www/css/style.scss www/css/style.min.css",
        "start": "http-server -o -c-1"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/BigstickCarpet/swagger-parser.git"
    },
    "devDependencies": {
        "bower": "^1.7.1",
        "chai": "^3.4.1",
        "coveralls": "^2.11.6",
        "eslint": "^1.10.3",
        "http-server": "^0.8.5",
        "istanbul": "^0.4.1",
        "jscs": "^2.7.0",
        "karma": "^0.13.16",
        "karma-chrome-launcher": "^0.2.2",
        "karma-cli": "^0.1.2",
        "karma-coverage": "^0.5.3",
        "karma-firefox-launcher": "^0.1.7",
        "karma-ie-launcher": "^0.2.0",
        "karma-mocha": "^0.2.1",
        "karma-phantomjs-launcher": "^0.2.2",
        "karma-safari-launcher": "^0.1.1",
        "karma-sauce-launcher": "^0.3.0",
        "karma-verbose-reporter": "0.0.3",
        "mocha": "^2.3.4",
        "node-sass": "^3.4.2",
        "npm-check-updates": "^2.5.6",
        "phantomjs": "^1.9.19",
        "simplifyify": "^2.0.1",
        "sinon": "^1.17.2",
        "superagent": "^1.6.1",
        "version-bump-prompt": "^1.5.2"
    },
    "dependencies": {
        "call-me-maybe": "^1.0.1",
        "debug": "^2.2.0",
        "es6-promise": "^3.0.2",
        "json-schema-ref-parser": "^1.4.1",
        "ono": "^2.0.1",
        "swagger-methods": "^1.0.0",
        "swagger-schema-official": "2.0.0-bab6bed",
        "z-schema": "^3.16.1"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
