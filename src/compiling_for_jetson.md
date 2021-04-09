---
title: Compiling Applications for the Jetson
---

# Environment Setup 

## Install cross-compiler toolchains

In order to cross-compile an appplication for the Nvidia Jetson Nano 2GB Developers Kit, the cross-compilers needed to be added to the path of the host machine.

Visit 
```
https://developer.nvidia.com/embedded/dlc/l4t-gcc-7-3-1-toolchain-64-bit
```

When downloaded, untar the file 

```
tar -xvf gcc-linaro-7.3.1-2018.05-x86_64_aarch64-linux-gnu.tar.xz
```

The binaries need to be added to the path

```
export PATH=./gcc-linaro-7.3.1-2018.05-x86_64_aarch64-linux-gnu/bin:$PATH
```

The cross-compilers are now available on the the path to be used.

## Cross-Compiling Application

Our application has a Makefile that allows it to be compiled for a specfic target architecture by defining the `CC` make variable on the command-line

`make all CC=aarch64-linux-gnu-gcc`

Once compiled, the exectuable is ready to be transferred to the board.