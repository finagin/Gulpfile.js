# Gulpfile.js
Gulpfile.js template

```bash
curl -sSL https://finagin.github.io/Gulpfile/init | sh
```

### Config file:
##### Gulpfile.json
```json
{
  "path": {
    "src": "./src",
    "root": "./",
    "dest": "./assets"
  },
  "proxy": {
    "path": "localhost",
    "port": 80
  }
}
```
* path.src - sources
* path.root - project root
* path.port - destination directory
* proxy.path - local url
* proxy.port - local port

### Gulp tasks
* default ["build", "watch"]
* build ["stylus", "js", "images"]