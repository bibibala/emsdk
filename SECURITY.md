
# init
```bash
./emsdk install latest
./emsdk activate latest
```


# start

```bash
source ./emsdk_env.sh
```


# run
```bash
emcc hello.c -o hello.html
```
```bash
emcc hello.c -o hello.js -s WASM=1 -O3 -m32
```


```bash
emcc hello.c -o output.js -s WASM=1 -s EXPORTED_RUNTIME_METHODS='["ccall", "cwrap"]'

```

```bash
emcc hello.c -o output.js -s WASM=1 -s EXPORTED_FUNCTIONS='["_add"]' -s EXPORTED_RUNTIME_METHODS='["ccall", "cwrap"]'
```