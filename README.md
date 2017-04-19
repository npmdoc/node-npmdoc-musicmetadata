# npmdoc-musicmetadata

#### api documentation for  [musicmetadata (v2.0.5)](https://github.com/leetreveil/musicmetadata#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-musicmetadata.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-musicmetadata) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-musicmetadata.svg)](https://travis-ci.org/npmdoc/node-npmdoc-musicmetadata)

#### Streaming music metadata parser for node and the browser.

[![NPM](https://nodei.co/npm/musicmetadata.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/musicmetadata)

- [https://npmdoc.github.io/node-npmdoc-musicmetadata/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-musicmetadata/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-musicmetadata/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-musicmetadata/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-musicmetadata/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-musicmetadata/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Lee Treveil"
    },
    "browser": "lib/browser",
    "bugs": {
        "url": "https://github.com/leetreveil/musicmetadata/issues"
    },
    "dependencies": {
        "deep-equal": "0.2.1",
        "filereader-stream": "^0.2.0",
        "is-stream": "^1.1.0",
        "strtok2": "~1.0.0",
        "through": "~2.3.4"
    },
    "description": "Streaming music metadata parser for node and the browser.",
    "devDependencies": {
        "brfs": "1.2.0",
        "browserify": "^13.0.0",
        "jshint": "~2.5.10",
        "standard": "^3.0.0",
        "tape": "^4.5.1",
        "testling": "^1.7.1"
    },
    "directories": {},
    "dist": {
        "shasum": "7ae910d99fbaee05f2bd543aef10b6fbe1f37bd4",
        "tarball": "https://registry.npmjs.org/musicmetadata/-/musicmetadata-2.0.5.tgz"
    },
    "engines": {
        "node": "*"
    },
    "gitHead": "90b8795756133ed9cdc5c1b85f7df48fbd983798",
    "homepage": "https://github.com/leetreveil/musicmetadata#readme",
    "jshintConfig": {
        "asi": true,
        "node": true,
        "maxlen": 100,
        "indent": 2
    },
    "keywords": [
        "id3",
        "id3v1",
        "id3v2",
        "m4a",
        "mp4",
        "vorbis",
        "ogg",
        "flac",
        "asf",
        "wma",
        "wmv",
        "tags",
        "tag"
    ],
    "license": "MIT",
    "main": "lib",
    "maintainers": [
        {
            "name": "leetreveil"
        }
    ],
    "name": "musicmetadata",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/leetreveil/musicmetadata.git"
    },
    "scripts": {
        "dist": "browserify lib/browser.js --standalone 'musicmetadata' -o dist/musicmetadata.js",
        "pretest": "standard && jshint lib/*.js test/*.js",
        "test": "[ ! -d 'test/' ] && echo 'The test directory is not included with the project due to the size of the test audio files. If you want to run the tests you can git clone the project.' || tape test/test-*.js",
        "test-browser": "for f in test/test-*.js; do browserify -t brfs $f | testling; done"
    },
    "standard": {
        "ignore": [
            "**/dist/**"
        ]
    },
    "testling": {
        "files": [
            "test/test-js-*.js",
            "test/js-*.js"
        ],
        "browsers": [
            "firefox/latest",
            "chrome/latest",
            "safari/latest"
        ]
    },
    "version": "2.0.5"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
