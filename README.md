## WIT
### Install cargo-component
```bash
$ cargo install cargo-component
```

### Create Project
```bash
$ cargo component new --lib greeter
```

### Build
```bash
$ cargo component build
```


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