# UnA
UnA is secure, scalable and absolutely decentralized cryptocurrency with adjustable level of confidentiality, created specifically for Africa.

To build UnA-Network:
1. Download the repository
2. Install dependencies
On Linux/Mac

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, and Boost 1.55.

You may download them from:

* http://gcc.gnu.org/
* http://www.cmake.org/
* http://www.boost.org/
* Alternatively, it may be possible to install them using a package manager.

On Windows
Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, and Boost 1.55. You may download them from:

* http://www.microsoft.com/
* http://www.cmake.org/
* http://www.boost.org/

3. Build

On Linux/Mac
Open una/cryptonote folder in terminal, and run `make`. The resulting executables can be found in `build/release/src`.

**Advanced options:**

* Parallel build: run `make -j<number of threads>` instead of `make`.
* Debug build: run `make build-debug`.
* Test suite: run `make test-release` to run tests in addition to building. Running `make test-debug` will do the same to the debug version.
* Building with Clang: it may be possible to use Clang instead of GCC, but this may not work everywhere. To build, run `export CC=clang CXX=clang++` before running `make`.

On Windows
 
* Open una/cryptonote folder in command prompt
* Run commands:
mkdir build
cd build
cmake -G "Visual Studio 12" .. (for 32-bit)
cmake -G "Visual Studio 12 Win64" .. (for64-bit)
Build created solution in Visual Studio

To build GUI UnA Wallet

1. Open una folder in command prompt/terminal
2. Run command:
mkdir build && cd build && cmake .. && make
