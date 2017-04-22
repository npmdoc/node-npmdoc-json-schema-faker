# npmdoc-json-schema-faker

#### api documentation for  [json-schema-faker (v0.4.1)](http://json-schema-faker.js.org)  [![npm package](https://img.shields.io/npm/v/npmdoc-json-schema-faker.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-json-schema-faker) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-json-schema-faker.svg)](https://travis-ci.org/npmdoc/node-npmdoc-json-schema-faker)

#### JSON-Schema + fake data generators

[![NPM](https://nodei.co/npm/json-schema-faker.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/json-schema-faker)

- [https://npmdoc.github.io/node-npmdoc-json-schema-faker/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-json-schema-faker/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-json-schema-faker/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-json-schema-faker/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-json-schema-faker/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-json-schema-faker/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/json-schema-faker/json-schema-faker/issues"
    },
    "contributors": [
        {
            "name": "Alvaro Cabrera"
        },
        {
            "name": "Tomasz Ducin",
            "url": "http://ducin.it"
        }
    ],
    "dependencies": {
        "chance": "^1.0.4",
        "deref": "^0.6.4",
        "faker": "3.0.1",
        "randexp": "^0.4.3"
    },
    "description": "JSON-Schema + fake data generators",
    "devDependencies": {
        "browserify": "^13.1.1",
        "casual": "^1.5.8",
        "clone": "^2.1.0",
        "codecov": "^1.0.1",
        "eslint": "^3.11.1",
        "fs-extra": "^1.0.0",
        "glob": "^7.1.1",
        "istanbul": "^0.4.5",
        "jasmine-node": "2.0.0-beta4",
        "jayschema": "^0.3.1",
        "lodash.template": "^4.4.0",
        "semver": "^5.3.0",
        "tslint": "^4.0.2",
        "tv4": "^1.2.7",
        "typedoc": "^0.5.1",
        "typescript": "^2.1.1",
        "uglify-js": "^2.7.4",
        "z-schema": "^3.18.1"
    },
    "directories": {},
    "dist": {
        "shasum": "3cfb15ab1355b88c05b9f4cc98555295dead3cf9",
        "tarball": "https://registry.npmjs.org/json-schema-faker/-/json-schema-faker-0.4.1.tgz"
    },
    "gitHead": "80302c07131ea0274ffc6f261c4683f26d5a25fc",
    "homepage": "http://json-schema-faker.js.org",
    "keywords": [
        "json",
        "jsonschema",
        "fake",
        "mocks"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "pateketrueke"
        },
        {
            "name": "ducin"
        }
    ],
    "name": "json-schema-faker",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/json-schema-faker/json-schema-faker.git"
    },
    "scripts": {
        "cover": "istanbul cover --root lib --x '**/spec/**' -- jasmine-node --coffee spec",
        "cover:up": "codecov --file=coverage/lcov.info --disable=gcov -e TRAVIS_NODE_VERSION",
        "dev": "jasmine-node spec/schema --coffee --verbose --autoTest --watchFolders lib",
        "dist": "node build/dist.js",
        "graphviz": "madge lib --dot > structure.gv",
        "test": "npm run test:lint && npm run test:unit && npm run test:schema",
        "test:lint": "tslint ts/**/*.ts && eslint lib",
        "test:schema": "jasmine-node spec/schema --coffee --noStackTrace --captureExceptions",
        "test:unit": "jasmine-node spec/unit --noStackTrace --captureExceptions",
        "tsc": "bash build/tsc.sh",
        "tsify": "browserify ts/index.ts -p [ tsify ] > dist/temp-bundle.js",
        "typedoc": "typedoc --out docs/html ts/ --module commonjs"
    },
    "version": "0.4.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
