# clion+ stm32 开发环境搭建
[参考jetbrains官方指导](https://www.jetbrains.com/help/clion/2021.2/embedded-development.html)
# 准备 

## 1. clion
## 2. gcc-arm-none-eabi
## 3. mingw-get-setup.exe
## 4. stm32cubemx-win.zip
## 5. OpenOCD  
### 5.1 openOCD 配置
配置ST-link烧写器配置文件
stm32f103_stlink.cfg
```config
source [find interface/stlink.cfg]
transport select hla_swd
source [find target/stm32f1x.cfg]
adapter speed 2000  // adapter_khz 2000
```
保存到openOCD脚本目录下：    
D:\WorkRoom\embedded\stm32\OpenOCD-20210729-0.11.0\share\openocd\scripts\board