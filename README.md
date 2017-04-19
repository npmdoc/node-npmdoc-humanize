# npmdoc-humanize

#### api documentation for  [humanize (v0.0.9)](https://github.com/taijinlee/humanize)  [![npm package](https://img.shields.io/npm/v/npmdoc-humanize.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-humanize) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-humanize.svg)](https://travis-ci.org/npmdoc/node-npmdoc-humanize)

#### Javascript string formatter for human readability

[![NPM](https://nodei.co/npm/humanize.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/humanize)

- [https://npmdoc.github.io/node-npmdoc-humanize/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-humanize/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-humanize/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-humanize/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-humanize/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-humanize/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tai-Jin Lee"
    },
    "bugs": {
        "url": "https://github.com/taijinlee/humanize/issues"
    },
    "dependencies": {},
    "description": "Javascript string formatter for human readability",
    "devDependencies": {
        "jshint": "0.7.1",
        "mocha": "1.0.3",
        "should": "0.6.3"
    },
    "directories": {},
    "dist": {
        "shasum": "1994ffaecdfe9c441ed2bdac7452b7bb4c9e41a4",
        "tarball": "https://registry.npmjs.org/humanize/-/humanize-0.0.9.tgz"
    },
    "engines": {
        "node": "*"
    },
    "homepage": "https://github.com/taijinlee/humanize",
    "keywords": [
        "util",
        "client",
        "browser"
    ],
    "main": "humanize.js",
    "maintainers": [
        {
            "name": "taijin"
        }
    ],
    "name": "humanize",
    "optionalDependencies": {},
    "readmeFilename": "README.md",
    "repository": {
        "type": "git",
        "url": "git://github.com/taijinlee/humanize.git"
    },
    "scripts": {
        "test": "./node_modules/jshint/bin/hint humanize.js; find specs -type f -a -name *.spec.js -exec ./node_modules/mocha/bin/mocha --globals requirejsVars -R list --require should {} \\;"
    },
    "version": "0.0.9"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
