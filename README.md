# Gulpfile.js
Gulpfile.js template

```bash
curl -sSL https://finagin.gihub.io/Gulpfile/init | sh
```

### Config file:
##### ./Gulpfile.json
```json
{
  "path": {
    "src": "./src",       // sources
    "root": "./",         // project root
    "dest": "./assets"    // destination directory
  },
  "proxy": {
    "path": "localhost",  // local url
    "port": 80            // local port
  }
}
```

### Gulp tasks
* default ["build", "watch"]
* build ["stylus", "js", "images"]