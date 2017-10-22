# Install protobuf
## prerequisites:
```
$ sudo apt-get install autoconf automake libtool curl make g++ unzip
```
## Installation steps:
```
$ ./autogen.sh
$ ./configure
$ make
$ make check
$ sudo make install
$ sudo ldconfig # refresh shared library cache.
```
# Install grpc(c++)
## prerequisites:
```
$ [sudo] apt-get install build-essential autoconf libtool
$ [sudo] apt-get install libgflags-dev libgtest-dev
$ [sudo] apt-get install clang libc++-dev
```
## Installation steps:
```
$ git clone -b $(curl -L https://grpc.io/release) https://github.com/grpc/grpc
$ cd grpc
$ git submodule update --init
$ make
$ [sudo] make install
```
