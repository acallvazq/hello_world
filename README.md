# WebAssembly Tutorial

This is a simple project I made while following a WebAssembly tutorial.
It compiles a basic C program to WebAssembly using Emscripten and runs it in the browser via JavaScript and HTML.

## 🚀 How to run

### HTTP Server
```
python3 -m http.server
```

### Compile
```
emcc hello_world.c

```
```
emcc wrapping.c -o wrapping.js

```


### Wrapping
```
emcc wrapping.c -o wrapping.js -s NO_EXIT_RUNTIME=1 -s EXPORTED_RUNTIME_METHODS=[ccall,cwrap]

```

