# pico-c

Contains two Pico projects: `Pico-Ultrasonic` and `pico-examples`.
Make sure you get `cmake` and `arm` compilers etc.
```
sudo apt update
sudo apt install gcc-arm-none-eabi libnewlib-arm-none-eabi build-essential libssl-dev tk tkinter python3-tk
```
You would need the [pico-sdk](https://github.com/raspberrypi/pico-sdk) as a submodule.
Please create build folders separately. For example, 
```
git submodule add https://github.com/raspberrypi/pico-sdk pico-sdk
cd pico-c
mkdir build
cd build
cmake ..
make
```
Youshould expect to have now `hello.elf` to load via a debugger, or `hello.uf2` that can be installed and run on 
your Raspberry Pi Pico via drag and drop.
