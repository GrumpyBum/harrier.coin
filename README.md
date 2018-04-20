Referance for Building Harrier.Coin Harraier Tech Project Daemon's and Miners.
Harrier Coin is been built for Ubuntu Linux and Windows Operating Systems and is Managed by http://harrier.tech
In building Harrier Coin please be aware of the Harrier GUI Wallet, https://github.com/GrumpyBum/harrier.wallet

## Building Harrier.Coin 

### On Ubuntu 16.04 LTS

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, and Boost 1.58.

You may download them from:

* http://gcc.gnu.org/
* http://www.cmake.org/
* http://www.boost.org/
* Or 'apt-get install build-essential cmake libboost1.58-all-dev'

To build, change to a directory where this file is located, and run `make`. The resulting executables can be found in `build/release/src`.

**Advanced options:**

* Parallel build: run `make -j<number of threads>` instead of `make`.
* Debug build: run `make build-debug`.
* Test suite: run `make test-release` to run tests in addition to building. Running `make test-debug` will do the same to the debug version.
* Building with Clang: it may be possible to use Clang instead of GCC, but this may not work everywhere. To build, run `export CC=clang CXX=clang++` before running `make`.

### On Windows
Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, Boost 1.55, Python 2.7.14, and QT5.0.2 (For GUI Wallet Only). You may download them from:

* http://www.microsoft.com/
* http://www.cmake.org/
* http://www.boost.org/

For GUI Functionality of Harrier Coin, CLI will build fine without the following:
* https://www.python.org
* https://www.qt.io/

To build, change to a directory where this file is located, and run theas commands: 
```
mkdir build
cd build
cmake -G "Visual Studio 12 Win64" ..
```
Once built the build directory is available to be compiled in Visual Studio 2013

And then do Build.
Good luck!
