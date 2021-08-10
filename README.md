# mcpelauncher-extract
Apk extraction utility/library for mcpelauncher-linux
# Information
This is a small utility which can be used to extract APKs for use with
mcpelauncher.
# Usage
```
mcpelauncher-extract <apk-file> [<apk-file>+] <destination>
```
# Building
## Dependencies
- Standard Build Tools
- [CMake](https://cmake.org/)
- [libzip](https://libzip.org/) (`libzip-dev` package on Debian/Ubuntu)
## Compiling
1. Retrieve the source:
```
git clone https://github.com/TheSonicMaster/mcpelauncher-extract
cd mcpelauncher-extract
```
2. Building:

- **Note: First install the dependencies above.**

```
mkdir -p build && cd build
cmake -DCMAKE_BUILD_TYPE=Release -Wno-dev ..
make
```
3. Running/Installing:

Executable is placed in the current directory, run it with:
```
./mcpelauncher-extract
```
OR install it system wide (default: `/usr/local/bin`) with:
```
sudo make install
```
And then run it with:
```
mcpelauncher-extract
```
