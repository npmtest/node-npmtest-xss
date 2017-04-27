# npmtest-xss

#### basic test coverage for  [xss (v0.3.3)](https://github.com/leizongmin/js-xss)  [![npm package](https://img.shields.io/npm/v/npmtest-xss.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-xss) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-xss.svg)](https://travis-ci.org/npmtest/node-npmtest-xss)

#### Sanitize untrusted HTML (to prevent XSS) with a configuration specified by a Whitelist

[![NPM](https://nodei.co/npm/xss.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/xss)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-xss/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-xss/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-xss/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-xss/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-xss/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-xss/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-xss/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-xss/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-xss/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-xss/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-xss/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-xss/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-xss/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-xss/build/test-report.html](https://npmtest.github.io/node-npmtest-xss/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-xss/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-xss/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-xss/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-xss/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-xss/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-xss/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-xss/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-xss/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Zongmin Lei",
        "url": "http://ucdok.com"
    },
    "bin": {
        "xss": "./bin/xss"
    },
    "bugs": {
        "url": "https://github.com/leizongmin/js-xss/issues"
    },
    "contributors": [
        {
            "name": "Zongmin Lei",
            "url": "http://ucdok.com"
        }
    ],
    "dependencies": {
        "commander": "^2.9.0",
        "cssfilter": "0.0.9"
    },
    "description": "Sanitize untrusted HTML (to prevent XSS) with a configuration specified by a Whitelist",
    "devDependencies": {
        "browserify": "^13.0.1",
        "coveralls": "^2.11.9",
        "debug": "^2.2.0",
        "istanbul": "^0.4.3",
        "mocha": "^3.0.2",
        "uglify-js": "^2.6.1"
    },
    "directories": {},
    "dist": {
        "shasum": "a014360dee10317331f9e74258141f7ed03fc784",
        "tarball": "https://registry.npmjs.org/xss/-/xss-0.3.3.tgz"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "files": [
        "lib",
        "bin/xss",
        "dist",
        "typings/*.d.ts"
    ],
    "gitHead": "18e0258ff2d9ecfd8bc99e83cc0c52ea8a28caea",
    "homepage": "https://github.com/leizongmin/js-xss",
    "keywords": [
        "sanitization",
        "xss",
        "sanitize",
        "sanitisation",
        "input",
        "security",
        "escape",
        "encode",
        "filter",
        "validator",
        "html",
        "injection",
        "whitelist"
    ],
    "license": "MIT",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "leizongmin"
        }
    ],
    "name": "xss",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/leizongmin/js-xss.git"
    },
    "scripts": {
        "build": "./bin/build",
        "prepublish": "npm run test && npm run build",
        "test": "export DEBUG=xss:* && mocha -t 5000",
        "test-cov": "export DEBUG=xss:* && istanbul cover _mocha --report lcovonly -- -t 5000 -R spec && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js && rm -rf ./coverage"
    },
    "typings": "./typings/xss.d.ts",
    "version": "0.3.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
