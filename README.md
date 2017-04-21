# npmtest-cnpmjs.org

#### basic test coverage for  [cnpmjs.org (v2.19.4)](https://github.com/cnpm/cnpmjs.org)  [![npm package](https://img.shields.io/npm/v/npmtest-cnpmjs.org.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-cnpmjs.org) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-cnpmjs.org.svg)](https://travis-ci.org/npmtest/node-npmtest-cnpmjs.org)

#### Private npm registry and web for Enterprise, base on MySQL and Simple Store Service

[![NPM](https://nodei.co/npm/cnpmjs.org.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cnpmjs.org)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-cnpmjs.org/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-cnpmjs.org/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-cnpmjs.org/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-cnpmjs.org/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-cnpmjs.org/build/test-report.html](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-cnpmjs.org/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-cnpmjs.org/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cnpmjs.org/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cnpmjs.org/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-cnpmjs.org/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "cnpmjs.org",
    "version": "2.19.4",
    "description": "Private npm registry and web for Enterprise, base on MySQL and Simple Store Service",
    "main": "index.js",
    "scripts": {
        "dev": "DEBUG=cnpm* node dispatch.js",
        "test": "make jshint && make test",
        "start": "./bin/nodejsctl start && cp History.md docs/web/history.md",
        "status": "./bin/nodejsctl status",
        "stop": "./bin/nodejsctl stop"
    },
    "bin": {
        "cnpmjs.org": "bin/cli.js"
    },
    "dependencies": {
        "agentkeepalive": "^2.2.0",
        "await-event": "^1.0.0",
        "bytes": "^2.4.0",
        "cfork": "^1.5.1",
        "changes-stream": "^1.1.0",
        "co": "^4.6.0",
        "co-defer": "^1.0.0",
        "co-gather": "^0.0.1",
        "co-sleep": "^0.0.1",
        "commander": "^2.9.0",
        "copy-to": "^2.0.1",
        "debug": "^2.2.0",
        "error-formater": "^1.0.3",
        "fs-cnpm": "^1.2.0",
        "giturl": "^1.0.0",
        "graceful": "^1.0.0",
        "gravatar": "^1.5.0",
        "humanize-ms": "^1.2.0",
        "humanize-number": "^0.0.2",
        "is-type-of": "^1.0.0",
        "kcors": "^1.2.1",
        "koa": "^1.2.0",
        "koa-limit": "^1.0.2",
        "koa-markdown": "^2.0.1",
        "koa-maxrequests": "^1.0.0",
        "koa-middlewares": "^2.1.0",
        "koa-mock": "^1.6.1",
        "koa-safe-jsonp": "^0.3.1",
        "markdown-it": "^3.0.6",
        "mime": "^1.3.4",
        "mini-logger": "^1.1.1",
        "mkdirp": "^0.5.0",
        "moment": "^2.12.0",
        "mysql": "^2.10.2",
        "mz": "^2.4.0",
        "nodemailer": "^1.3.0",
        "normalize-registry-metadata": "^1.1.2",
        "semver": "^5.2.0",
        "sequelize": "^3.23.4",
        "thunkify-wrap": "^1.0.4",
        "treekill": "^1.0.0",
        "tunnel-agent": "^0.4.0",
        "urllib": "^2.11.0",
        "utility": "^1.8.0",
        "xss": "^0.2.13"
    },
    "devDependencies": {
        "autod": "*",
        "chunkstream": "*",
        "contributors": "*",
        "istanbul": "*",
        "jshint": "*",
        "mm": "*",
        "mocha": "*",
        "node-dev": "*",
        "pedding": "*",
        "pg": "5",
        "pg-hstore": "2",
        "should": "8",
        "sqlite3": "*",
        "supertest": "2",
        "thunk-mocha": "1"
    },
    "homepage": "https://github.com/cnpm/cnpmjs.org",
    "repository": {
        "type": "git",
        "url": "git://github.com/cnpm/cnpmjs.org.git",
        "web": "https://github.com/cnpm/cnpmjs.org"
    },
    "bugs": {
        "url": "https://github.com/cnpm/cnpmjs.org/issues"
    },
    "keywords": [
        "cnpmjs.org",
        "npm",
        "npmjs",
        "npmjs.org",
        "registry"
    ],
    "engines": {
        "node": ">= 4.3.1"
    },
    "author": [
        "fengmk2 <fengmk2@gmail.com> (http://fengmk2.com)",
        "dead_horse <dead_horse@qq.com> (http://deadhorse.me)"
    ],
    "license": "MIT"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
