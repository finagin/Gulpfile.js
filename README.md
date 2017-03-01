# Gulpfile.js
Gulpfile.js template


## Installation
```bash
curl -sSL finagin.github.io/Gulpfile | sh [-s -- -h]
```
or last version without cache
```bash
curl -sSL rawgit.com/finagin/Gulpfile.js/master/init | sh [-s -- -h]
```

### Config file:
##### Gulpfile.json
```json
{
    "path": {
        "src": "./src",
        "root": "./",
        "dist": "./assets/"
    },
    "proxy": {
        "protocol": "http://",
        "path": "localhost",
        "port": 8888
    },
    "gitignore": true
}
```
* path {Object} - paths list
    * path.src {String} - sources
    * path.root {String} - project root
    * path.dist {String} - destination directory
* proxy {Object | False} - proxy params
    * proxy.protocol {String} - local protocol
    * proxy.path {String} - local url
    * proxy.port {Integer} - local port
* gitignore {Boolean} - adding dist to .gitignore

### Gulp tasks
* default ["build", "watch"]
* build ["stylus", "js", "other"]

## Structure
### SRC
```$xslt
src/
├── fonts/
│   ├── .gitkeep
│   └── Ubuntu.ttf
├── js/
│   ├── separate/
│   │   ├── .gitkeep
│   │   ├── sepfile1.js
│   │   └── sepfile2.js
│   ├── file1.js
│   └── file2.js
└── stylus/
    ├── imports/
    │   └── .gitkeep
    ├── separate/
    │   ├── .gitkeep
    │   ├── sepfile1.styl
    │   └── sepfile2.styl
    ├── file1.styl
    └── file2.styl
```
### Dist
```$xslt
dist/
├── fonts/
│   └── Ubuntu.ttf
├── js/
│   ├── sepfile1.js
│   ├── sepfile2.js
│   └── main.js
└── css/
    ├── sepfile1.css
    ├── sepfile2.css
    └── style.css
```

## LICENSE
#### MIT License

Copyright (c) 2016 Igor Finagin

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
