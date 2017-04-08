# api documentation for  [realm (v1.2.0)](https://realm.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-realm.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-realm) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-realm.svg)](https://travis-ci.org/npmdoc/node-npmdoc-realm)
#### Realm is a mobile database: an alternative to SQLite and key-value stores

[![NPM](https://nodei.co/npm/realm.png?downloads=true)](https://www.npmjs.com/package/realm)

[![apidoc](https://npmdoc.github.io/node-npmdoc-realm/build/screenCapture.buildNpmdoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-realm%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-realm/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-realm/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-realm/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Realm",
        "email": "help@realm.io",
        "url": "https://realm.io"
    },
    "binary": {
        "module_name": "realm",
        "module_path": "./compiled/{node_abi}_{platform}_{arch}/",
        "host": "https://static.realm.io",
        "remote_path": "/node-pre-gyp"
    },
    "bugs": {
        "url": "https://github.com/realm/realm-js/issues"
    },
    "dependencies": {
        "extract-zip": "^1.6.0",
        "ini": "^1.3.4",
        "nan": "^2.3.3",
        "node-fetch": "^1.6.3",
        "node-pre-gyp": "^0.6.30",
        "request": "^2.78.0",
        "sync-request": "^3.0.1",
        "url-parse": "^1.1.7"
    },
    "description": "Realm is a mobile database: an alternative to SQLite and key-value stores",
    "devDependencies": {
        "babel-eslint": "^6.0.4",
        "eslint": "^3.2.2",
        "eslint-plugin-jasmine": "^2.1.0",
        "eslint-plugin-react": "^6.7.0",
        "jsdoc": "^3.4.0",
        "license-checker": "^8.0.3",
        "mockery": "^2.0.0",
        "rimraf": "^2.6.1",
        "semver": "^5.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "1f4531e86cd7f7e5219d6024fd4c46ae50ad4c2d",
        "tarball": "https://registry.npmjs.org/realm/-/realm-1.2.0.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "files": [
        "android",
        "lib",
        "react-native",
        "scripts",
        "src",
        "tests",
        "vendor",
        "binding.gyp",
        "realm.gypi",
        "target_defaults.gypi",
        "dependencies.list"
    ],
    "gitHead": "92c10c469c5d92c4044d953e9167afa477dc687c",
    "homepage": "https://realm.io",
    "keywords": [
        "database",
        "db",
        "react",
        "react-native",
        "persistence",
        "localstorage",
        "sqlite",
        "asyncstorage",
        "rocksdb",
        "leveldb",
        "realm"
    ],
    "license": "Apache-2.0",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "realmnpm",
            "email": "km@realm.io"
        }
    ],
    "name": "realm",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/realm/realm-js.git"
    },
    "rnpm": {
        "ios": {
            "project": "react-native/ios/RealmReact.xcodeproj",
            "sharedLibraries": [
                "libc++",
                "libz"
            ]
        }
    },
    "scripts": {
        "eslint": "npm install && npm run lint .",
        "get-core-version": "scripts/download-core.sh --version",
        "get-sync-version": "scripts/download-core.sh --versionSync",
        "get-version": "node -p process.env.npm_package_version",
        "install": "node-pre-gyp install --fallback-to-build",
        "isMac": "node -p \"if (process.platform == 'darwin') { process.exit(0); } else { process.exit(-1); }\"",
        "jsdoc": "npm install && npm run jsdoc:clean && jsdoc -c docs/conf.json",
        "jsdoc:clean": "rimraf ./docs/output",
        "license-check": "npm install && license-checker --exclude \"MIT,ISC,BSD,Apache-2.0,BSD-2-Clause,BSD-3-Clause,WTFPL,Unlicense,(MIT AND CC-BY-3.0)\" | node scripts/handle-license-check.js",
        "lint": "eslint",
        "node-nosync-tests": "npm install --build-from-source && cd tests && npm install && npm run test-nosync && cd ..",
        "node-tests": "npm install --build-from-source && cd tests && npm install && npm run test-nosync && cd ..",
        "prepublish": "node scripts/prepublish.js",
        "set-version": "scripts/set-version.sh",
        "test": "scripts/test.sh",
        "test-runner:ava": "cd tests/test-runners/ava && npm install && npm test",
        "test-runner:jest": "cd tests/test-runners/jest && npm install && npm test",
        "test-runner:mocha": "cd tests/test-runners/mocha && npm install && npm test",
        "test-runners": "npm run test-runner:ava && npm run test-runner:mocha && npm run test-runner:jest",
        "testMac": "npm run isMac -s && echo this is mac || echo . "
    },
    "version": "1.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module realm](#apidoc.module.realm)
1.  object <span class="apidocSignatureSpan">realm.</span>errors

#### [module realm.errors](#apidoc.module.realm.errors)
1.  [function <span class="apidocSignatureSpan">realm.errors.</span>AuthError (problem)](#apidoc.element.realm.errors.AuthError)



# <a name="apidoc.module.realm"></a>[module realm](#apidoc.module.realm)



# <a name="apidoc.module.realm.errors"></a>[module realm.errors](#apidoc.module.realm.errors)

#### <a name="apidoc.element.realm.errors.AuthError"></a>[function <span class="apidocSignatureSpan">realm.errors.</span>AuthError (problem)](#apidoc.element.realm.errors.AuthError)
- description and source-code
```javascript
function AuthError(problem) {
    Error.call(this, problem.title);
    Object.assign(this, problem);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
