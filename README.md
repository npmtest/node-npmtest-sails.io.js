# npmtest-sails.io.js

#### basic test coverage for  [sails.io.js (v1.1.10)](https://github.com/balderdashy/sails.io.js)  [![npm package](https://img.shields.io/npm/v/npmtest-sails.io.js.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-sails.io.js) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-sails.io.js.svg)](https://travis-ci.org/npmtest/node-npmtest-sails.io.js)

#### Javascript SDK for communicating w/ a Sails server via WebSockets/socket.io.

[![NPM](https://nodei.co/npm/sails.io.js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/sails.io.js)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-sails.io.js/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-sails.io.js/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-sails.io.js/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-sails.io.js/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-sails.io.js/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-sails.io.js/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-sails.io.js/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-sails.io.js/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-sails.io.js/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-sails.io.js/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-sails.io.js/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-sails.io.js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-sails.io.js/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-sails.io.js/build/test-report.html](https://npmtest.github.io/node-npmtest-sails.io.js/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-sails.io.js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-sails.io.js/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-sails.io.js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-sails.io.js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sails.io.js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sails.io.js/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-sails.io.js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-sails.io.js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mike McNeil",
        "url": "http://balderdash.co/"
    },
    "bugs": {
        "url": "https://github.com/balderdashy/sails.io.js/issues"
    },
    "dependencies": {
        "socket.io-client": "1.7.3"
    },
    "description": "Javascript SDK for communicating w/ a Sails server via WebSockets/socket.io.",
    "devDependencies": {
        "async": "2.0.1",
        "fs-extra": "0.30.0",
        "grunt": "1.0.1",
        "grunt-cli": "1.2.0",
        "grunt-contrib-clean": "1.0.0",
        "grunt-contrib-concat": "1.0.1",
        "grunt-contrib-copy": "1.0.0",
        "grunt-contrib-uglify": "1.0.1",
        "grunt-contrib-watch": "1.0.0",
        "grunt-text-replace": "0.4.0",
        "lodash": "3.10.1",
        "mocha": "3.0.2",
        "phantomjs-prebuilt": "2.1.12",
        "request": "2.74.0",
        "sails": "^1.0.0-16",
        "sails-hook-sockets": "^1.2.3",
        "socket.io-client": "1.7.2"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "86f8e81cc1b115c943fb532a53b57c97e3b895cf",
        "tarball": "https://registry.npmjs.org/sails.io.js/-/sails.io.js-1.1.10.tgz"
    },
    "gitHead": "375f154c652e5acc4b89b7bd9cf87bc67a10ff93",
    "homepage": "https://github.com/balderdashy/sails.io.js",
    "keywords": [
        "sails",
        "sdk",
        "sails.io.js",
        "socket.io",
        "browser",
        "javascript"
    ],
    "license": "MIT",
    "main": "sails.io.js",
    "maintainers": [
        {
            "name": "balderdashy"
        },
        {
            "name": "sgress454"
        },
        {
            "name": "particlebanana"
        },
        {
            "name": "mikermcneil"
        }
    ],
    "name": "sails.io.js",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/balderdashy/sails.io.js.git"
    },
    "scripts": {
        "postpublish": "cd dist && npm publish && cd .. && echo && echo '--' && echo 'Now, assuming you have not pushed up your automatic \"npm version\" commit+tag yet, run:' && echo \"git tag -d v'npm show sails.io.js version' && git commit --amend -am ''npm show sails.io.js version'' && git tag v'npm show sails.io.js version'\" && echo 'Then do:' && echo 'git push && git push --tags'",
        "prepublish": "./node_modules/grunt-cli/bin/grunt publish",
        "test": "node ./node_modules/mocha/bin/mocha -b --reporter spec --timeout 10000"
    },
    "version": "1.1.10",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
