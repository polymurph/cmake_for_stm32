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

## common problems

### already existing .zip files error When generating code with STM32CubeMX
when generating the code inside Project go to the section Mcu and Firmware Package.
Copy the link under Use Default Firmware location. Delete the problematic .zip file
(e.g. stm32cube_fw_f0_v1110.zip) and retry generating code.

## source
project idea is based on:
https://dev.to/younup/cmake-on-stm32-the-beginning-3766
