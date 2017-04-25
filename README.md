# npmtest-oneapm

#### basic test coverage for  [oneapm (v2.0.0)](http://oneapm.com/features/nodejs.html)  [![npm package](https://img.shields.io/npm/v/npmtest-oneapm.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-oneapm) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-oneapm.svg)](https://travis-ci.org/npmtest/node-npmtest-oneapm)

#### OneAPM agent

[![NPM](https://nodei.co/npm/oneapm.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/oneapm)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-oneapm/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-oneapm/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-oneapm/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-oneapm/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-oneapm/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-oneapm/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-oneapm/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-oneapm/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-oneapm/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-oneapm/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-oneapm/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-oneapm/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-oneapm/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-oneapm/build/test-report.html](https://npmtest.github.io/node-npmtest-oneapm/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-oneapm/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-oneapm/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-oneapm/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-oneapm/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-oneapm/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-oneapm/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-oneapm/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-oneapm/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "oneapm",
    "version": "2.0.0",
    "author": "OneAPM Node.js agent team <nodejs@oneapm.com>",
    "description": "OneAPM agent",
    "keywords": [
        "apm",
        "performance",
        "monitoring",
        "instrumentation",
        "debugging",
        "profiling"
    ],
    "homepage": "http://oneapm.com/features/nodejs.html",
    "engines": {
        "node": ">=0.10.0"
    },
    "directories": {
        "lib": "lib"
    },
    "scripts": {
        "plato": "./node_modules/.bin/plato -r -d dist/plato lib/**/*.js lib/*.js index.js oneapm.js",
        "tarball": "./bin/tarball.sh",
        "test": "mocha --no-deprecation",
        "test-cov": "istanbul cover node_modules/mocha/bin/_mocha --report html -- --check-leaks test/",
        "test-ci": "istanbul cover node_modules/mocha/bin/_mocha --report cobertura -- --reporter xunit --reporter-options output=coverage/junit.xml test/"
    },
    "dependencies": {
        "bunyan": "0.14.6",
        "continuation-local-storage": "^3.1.0",
        "debug": "^2.1.3",
        "is-docker": "^1.0.0",
        "oneapm-config": "^1.0.0",
        "oneapm-logger": "^2.0.0",
        "oneapm-server": "^1.0.0",
        "oneapm-util": "^1.0.0",
        "pidusage-fork": "^0.1.1",
        "semver": "^4.3.6"
    },
    "files": [
        "api.js",
        "CHANGELOG.md",
        "index.js",
        "lib/",
        "locales.js",
        "oneapm.js",
        "README.md",
        "stub_api.js"
    ],
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
