Aleksei Prokopov prepared this project for Embeetle IDE:
https://github.com/roboter/Hardware/tree/main/STM32/STM32F429-Discovery/embeetle/lv_port_stm32f429_disco

The [STM32F429 Discovery kit](https://www.st.com/en/evaluation-tools/32f429idiscovery.html) is an
affordable development board with:
* 240x320 (QVGA) TFT
* Resistive touchscreen
* 180 MHz MCU
* 256KB RAM
* 64-MBit SDRAM
* GPU.

The CubeMX drivers are used to initilaize the peripherals. In 'hal_stm_lvgl/tft/tft.h' you can
enable/disable external frame buffer placement and GPU usage. The project was created with CubeIDE.

Get started:
- Clone the project:
    `git clone https://github.com/littlevgl/stm32f429_disco_no_os_sw4stm32.git --recurse-submodules`
- Import into CubeIDE

Note:
It's important to add the -DSTM32F4 flag to the TARGET_CFLAGS and
TARGET_CXXFLAGS in '<project>/config/dashboard.mk' such that LVGL
works properly.