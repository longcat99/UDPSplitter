https://github.com/OpenHD/OpenHD/tree/nightly-2020-1-23/UDPSplitter
```
sudo apt-get install build-essential
sudo apt install gcc-arm-linux-gnueabihf g++-arm-linux-gnueabihf
sudo apt install cmake
cmake -DCMAKE_TOOLCHAIN_FILE=toolchain-arm-linux.cmake -B build -S .
cd build
make
```
