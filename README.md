# npmtest-swagger-parser

#### basic test coverage for  [swagger-parser (v3.4.1)](https://bigstickcarpet.github.io/swagger-parser)  [![npm package](https://img.shields.io/npm/v/npmtest-swagger-parser.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-swagger-parser) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-swagger-parser.svg)](https://travis-ci.org/npmtest/node-npmtest-swagger-parser)

#### Swagger 2.0 parser and validator for Node and browsers

[![NPM](https://nodei.co/npm/swagger-parser.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/swagger-parser)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-swagger-parser/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-swagger-parser/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-swagger-parser/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-swagger-parser/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-swagger-parser/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-swagger-parser/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-swagger-parser/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-swagger-parser/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-swagger-parser/tree/gh-pages/build)|

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
    "author": {
        "name": "James Messinger",
        "url": "http://jamesmessinger.com"
    },
    "bugs": {
        "url": "https://github.com/BigstickCarpet/swagger-parser/issues"
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
    },
    "description": "Swagger 2.0 parser and validator for Node and browsers",
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
    "directories": {},
    "dist": {
        "shasum": "0290529dbae254d178b442a95df60d23d142301d",
        "tarball": "https://registry.npmjs.org/swagger-parser/-/swagger-parser-3.4.1.tgz"
    },
    "gitHead": "efffb4cc66c9be9fb78bc6b69b33fc2fd2290e66",
    "homepage": "https://bigstickcarpet.github.io/swagger-parser",
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
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "bigstickcarpet"
        },
        {
            "name": "rkrauskopf"
        }
    ],
    "name": "swagger-parser",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/BigstickCarpet/swagger-parser.git"
    },
    "scripts": {
        "browserify": "simplifyify lib/index.js --outfile dist/swagger-parser.js --standalone SwaggerParser --bundle --debug --minify",
        "browserify-www": "simplifyify www/js/index.js --outfile www/js/bundle.js --bundle --debug --minify",
        "build": "npm run lint && npm run browserify && npm run build-www",
        "build-www": "npm run sass && npm run browserify-www",
        "bump": "bump --prompt --grep lib/index.js dist/* --tag --push --all",
        "istanbul": "istanbul cover _mocha --dir coverage/node -- --bail --recursive tests/fixtures tests/specs",
        "karma": "karma start --single-run",
        "lint": "eslint lib && jscs lib --verbose",
        "mocha": "mocha --bail --async-only --recursive tests/fixtures tests/specs",
        "release": "npm run upgrade && npm run build-www && npm test && npm run bump && npm publish",
        "sass": "node-sass --source-map true --output-style compressed www/css/style.scss www/css/style.min.css",
        "start": "http-server -o -c-1",
        "test": "npm run browserify -- --test && npm run istanbul && npm run karma",
        "upgrade": "ncu --upgradeAll && npm update && bower update",
        "watch": "npm run browserify -- --watch & npm run browserify-www -- --watch"
    },
    "version": "3.4.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
