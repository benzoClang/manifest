benzoClang - Custom AOSP LLVM with Polly
------------------------

How to build:
```
$ mkdir benzoClang
$ cd benzoClang
$ repo init -u https://github.com/benzoClang/manifest -b master
$ repo sync -j$(nproc --all) -f
```

After syncing, for a quicker build run:
```
$ toolchain/llvm_benzo/build.py --no-lto
```
and to build using ThinLTO just run:
```
$ toolchain/llvm_benzo/build.py
```
But ThinLTO builds take a lot longer,
