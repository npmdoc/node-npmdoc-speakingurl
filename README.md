# api documentation for  [speakingurl (v13.0.0)](http://pid.github.io/speakingurl/)  [![npm package](https://img.shields.io/npm/v/npmdoc-speakingurl.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-speakingurl) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-speakingurl.svg)](https://travis-ci.org/npmdoc/node-npmdoc-speakingurl)
#### Generate a slug – transliteration with a lot of options

[![NPM](https://nodei.co/npm/speakingurl.png?downloads=true)](https://www.npmjs.com/package/speakingurl)

[![apidoc](https://npmdoc.github.io/node-npmdoc-speakingurl/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-speakingurl_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-speakingurl/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-speakingurl/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-speakingurl/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Sascha Droste",
        "email": "pid@posteo.net",
        "url": "https://twitter.com/SaschaDroste"
    },
    "bugs": {
        "url": "https://github.com/pid/speakingurl/issues"
    },
    "categories": [
        "Utilities",
        "Parsers & Compilers"
    ],
    "dependencies": {},
    "description": "Generate a slug – transliteration with a lot of options",
    "devDependencies": {
        "gulp": "^3.8.8",
        "gulp-bump": "^2.4.0",
        "gulp-header": "^1.2.2",
        "gulp-jsbeautifier": "^2.0.3",
        "gulp-jshint": "^2.0.0",
        "gulp-load-plugins": "^1.1.0",
        "gulp-mocha": "^3.0.1",
        "gulp-rename": "^1.2.0",
        "gulp-replace": "^0.5.0",
        "gulp-uglify": "^2.0.0",
        "jshint": "^2.8.0",
        "jshint-stylish": "^2.0.0",
        "minimist": "^1.1.0",
        "mocha": "^3.0.2",
        "should": "^11.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "266c52d2b47585375af058e4783c8d1097a2d3db",
        "tarball": "https://registry.npmjs.org/speakingurl/-/speakingurl-13.0.0.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "filename": "speakingurl.min.js",
    "gitHead": "31c5b7ce85a69a7721acd090f73235c97890a4a9",
    "github": "http://github.com/pid/speakingurl",
    "homepage": "http://pid.github.io/speakingurl/",
    "jam": {
        "dependencies": {},
        "main": "speakingurl.min.js",
        "shim": {
            "deps": [],
            "exports": [
                "getSlug",
                "createSlug"
            ]
        },
        "include": [
            "speakingurl.min.js",
            "README.md"
        ]
    },
    "keywords": [
        "slug",
        "slugify",
        "speakingurl",
        "transliteration",
        "permalink",
        "seo",
        "url",
        "nice url",
        "static url",
        "clean url",
        "pretty url",
        "nice looking url",
        "user friendly url",
        "seo friendly url"
    ],
    "license": "BSD-3-Clause",
    "licenses": [
        {
            "type": "BSD",
            "url": "https://raw.github.com/pid/speakingurl/master/LICENSE"
        }
    ],
    "main": "index",
    "maintainers": [
        {
            "name": "pid",
            "email": "sascha.droste@gmail.com"
        }
    ],
    "name": "speakingurl",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/%3Apid/speakingurl.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "version": "13.0.0",
    "volo": {
        "url": "//cdnjs.cloudflare.com/ajax/libs/speakingurl/{version}/speakingurl.min.js"
    }
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module speakingurl](#apidoc.module.speakingurl)
1.  [function <span class="apidocSignatureSpan">speakingurl.</span>createSlug (opts)](#apidoc.element.speakingurl.createSlug)



# <a name="apidoc.module.speakingurl"></a>[module speakingurl](#apidoc.module.speakingurl)

#### <a name="apidoc.element.speakingurl.createSlug"></a>[function <span class="apidocSignatureSpan">speakingurl.</span>createSlug (opts)](#apidoc.element.speakingurl.createSlug)
- description and source-code
```javascript
function createSlug(opts) {

<span class="apidocCodeCommentSpan">    /**
     * getSlugWithConfig
     * @param   {string} input string
     * @return  {string} slug string
     */
</span>    return function getSlugWithConfig(input) {
        return getSlug(input, opts);
    };
}
```
- example usage
```shell
...

'''js
var options = {
	    maintainCase: true,
	    separator: '_'
	};

var mySlug = require('speakingurl').createSlug(options);
// in browser:
// var mySlug = createSlug(options);

var slug = mySlug("Schöner Titel läßt grüßen!? Bel été !");
console.log(slug); // Output: Schoener_Titel_laesst_gruessen_Bel_ete
'''
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
