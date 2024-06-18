
## Host
### Prepare
In `./host/js`

Transplie  
```bash
$ jco transpile  ../../greeter/target/wasm32-wasi/debug/greeter.wasm -o greeter
```

Rename
```bash
$ mv greeter/greeter.js greeter/greeter.mjs
```

### Run
```bash
$ node index.mjs 
```