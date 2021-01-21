# cmake_for_stm32

## checking version of needed tools

Cmake version
```
cmake --version
```
arm gcc toolchain
```
arm-none-eabi-gcc --version
```

## setting up CMakeLists.txt

- copy the source .c/.h file directories in the CMakeLists.txt. 

## making the project C/C++

The '''main.c''' is the entry point of the project.
What is needed is funtion in which a main loop in C++ is called.
With creating a appMain.cpp/.hpp a wrapperfunction can be created which can be called from main.c.

## common problems

### already existing .zip files error When generating code with STM32CubeMX
when generating the code inside Project go to the section Mcu and Firmware Package.
Copy the link under Use Default Firmware location. Delete the problematic .zip file
(e.g. stm32cube_fw_f0_v1110.zip) and retry generating code.

## source
project idea is based on:
https://dev.to/younup/cmake-on-stm32-the-beginning-3766

arm compiler options
https://gcc.gnu.org/onlinedocs/gcc-4.4.7/gcc/ARM-Options.html

