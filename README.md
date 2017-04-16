# test coverage for  [immutable (v3.8.1)](https://facebook.github.com/immutable-js)  [![npm package](https://img.shields.io/npm/v/npmtest-immutable.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-immutable) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-immutable.svg)](https://travis-ci.org/npmtest/node-npmtest-immutable)
#### Immutable Data Collections

[![NPM](https://nodei.co/npm/immutable.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/immutable)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-immutable/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-immutable/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-immutable/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-immutable/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-immutable/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-immutable/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-immutable/tree/gh-pages/build)|

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-immutable/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-immutable/build/coverage.html/index.html)

[![test-report](https://npmtest.github.io/node-npmtest-immutable/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-immutable/build/test-report.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-immutable/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-immutable/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-immutable/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-immutable/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Lee Byron",
        "url": "https://github.com/leebyron"
    },
    "bugs": {
        "url": "https://github.com/facebook/immutable-js/issues"
    },
    "dependencies": {},
    "description": "Immutable Data Collections",
    "devDependencies": {
        "acorn": "0.11.x",
        "babel-eslint": "^4.1.8",
        "benchmark": "^1.0.0",
        "bluebird": "3.1.1",
        "browser-sync": "2.11.0",
        "browserify": "^5.11.2",
        "colors": "1.1.2",
        "del": "2.2.0",
        "es6-transpiler": "0.7.18",
        "eslint": "^1.10.3",
        "estraverse": "1.9.3",
        "express": "^4.13.4",
        "fbjs-scripts": "^0.5.0",
        "grunt": "0.4.5",
        "grunt-cli": "0.1.13",
        "grunt-contrib-clean": "0.7.0",
        "grunt-contrib-copy": "0.8.2",
        "grunt-contrib-jshint": "0.11.3",
        "grunt-release": "0.13.0",
        "gulp": "3.9.0",
        "gulp-concat": "2.6.0",
        "gulp-filter": "3.0.1",
        "gulp-header": "1.7.1",
        "gulp-jest": "^0.2.1",
        "gulp-jshint": "^1.8.4",
        "gulp-less": "3.0.5",
        "gulp-size": "2.0.0",
        "gulp-sourcemaps": "1.6.0",
        "gulp-uglify": "1.5.1",
        "gulp-util": "3.0.7",
        "harmonize": "1.4.4",
        "jasmine-check": "^0.1.2",
        "jest-cli": "^0.5.10",
        "jshint-stylish": "^0.4.0",
        "magic-string": "0.10.2",
        "marked": "0.3.5",
        "microtime": "^2.0.0",
        "node-jsx": "^0.12.4",
        "react": "^0.12.0",
        "react-router": "^0.11.2",
        "react-tools": "^0.12.0",
        "rollup": "0.24.0",
        "run-sequence": "1.1.5",
        "through2": "2.0.0",
        "typescript": "1.7.5",
        "uglify-js": "2.6.1",
        "vinyl-buffer": "1.0.0",
        "vinyl-source-stream": "1.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "200807f11ab0f72710ea485542de088075f68cd2",
        "tarball": "https://registry.npmjs.org/immutable/-/immutable-3.8.1.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "files": [
        "dist",
        "contrib",
        "README.md",
        "LICENSE",
        "PATENTS"
    ],
    "gitHead": "e96d73f7e1fbeff00d03b09aa4352e04de61abb3",
    "homepage": "https://facebook.github.com/immutable-js",
    "jest": {
        "scriptPreprocessor": "resources/jestPreprocessor.js",
        "testFileExtensions": [
            "js",
            "ts"
        ],
        "persistModuleRegistryBetweenSpecs": true
    },
    "keywords": [
        "immutable",
        "persistent",
        "lazy",
        "data",
        "datastructure",
        "functional",
        "collection",
        "stateless",
        "sequence",
        "iteration"
    ],
    "license": "BSD-3-Clause",
    "main": "dist/immutable.js",
    "maintainers": [
        {
            "name": "leebyron"
        }
    ],
    "name": "immutable",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/facebook/immutable-js.git"
    },
    "scripts": {
        "build": "grunt default && gulp default",
        "deploy": "(cd ./pages/out && git init && git config user.name \"Travis CI\" && git config user.email \"github@fb.com\" && git add . && git commit -m \"Deploy to GitHub Pages\" && git push --force --quiet \"https://${GH_TOKEN}@github.com/facebook/immutable-js.git\" master:gh-pages > /dev/null 2>1)",
        "lint": "eslint src/ && grunt lint && gulp lint",
        "perf": "node ./resources/bench.js",
        "start": "npm run build && node ./pages/resources/start.js",
        "test": "npm run lint && npm run testonly",
        "testonly": "./resources/node_test.sh"
    },
    "typescript": {
        "definition": "dist/immutable.d.ts"
    },
    "typings": "dist/immutable-nonambient.d.ts",
    "version": "3.8.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
