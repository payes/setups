# Install protobuf
## prerequisites:
```
$ sudo apt-get install autoconf automake libtool curl make g++ unzip
```
## Installation steps:
```
$ git clone https://github.com/google/protobuf.git
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
$ [sudo] apt-get install build-essential autoconf libtool libgflags-dev libgtest-dev clang libc++-dev
```
## Installation steps:
```
$ git clone -b $(curl -L https://grpc.io/release) https://github.com/grpc/grpc
$ cd grpc
$ git submodule update --init
$ make
$ [sudo] make install
```
# Install yaml-cpp
## prerequisites:
```
$ [sudo] apt-get install cmake
```
## Installation steps:
```
$ git clone https://github.com/jbeder/yaml-cpp.git
$ cd yaml-cpp
$ makir build
$ cd src
$ cmake -DBUILD_SHARED_LIBS=ON ..
$ sudo make install
```
