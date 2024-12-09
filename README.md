# Static Qt builds

Currently this only contains static builds of Qt for macOS.

## Building for

# macOS

Qt version: 6.5.3

```
./configure -static -submodules qt5compat,qtshadertools,qtimageformats,qtmultimedia,qtremoteobjects,qttools,qtdeclarative,qtsvg -prefix $(pwd)/deploy -- -DCMAKE_OSX_ARCHITECTURES="x86_64"
cmake --build . --parallel
```

