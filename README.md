<div align="center">

# Free-DAP

<img height=300 title="Logo by GPT-5" src="./logo.png"/>
<br/>
<br/>

This is a specialized version of Alex Taradov's implementation of the CMSIS-DAP debugger firmware for use with the [RPDAP](https://github.com/ruben-iteng/RPDAP) hardware.

</div>

## Features

- CMSIS-DAP v2
- SWD
- JTAG
- UART VCP (Virtual COM Port)
- Bi-directional level shifter support (direction pin control)

## Binaries

Binaries are automatically built and added to the [releases](https://github.com/ruben-iteng/Free-DAP/releases/latest).
Just download the uf2 file, put your RP2040 into boot mode (hold the boot button while plugging in the USB cable) and copy the file to the RP2040 drive. It will automatically reboot into the new firmware.

## Pinout

The default RP2040 pinout:

| GPIO | Function |
|:---:|:---|
| 11 | SWCLK/TCK |
| 12 | SWDIO/TMS |
| 13 | TDI |
| 14 | TDO |
| 15 | nRESET |
| 0 | VCP TX |
| 1 | VCP RX |
| 2 | VCP Status (LED)|
| 25 | DAP Status (LED)|
| 9 | Direction (DIO/TMS level shifter)|
