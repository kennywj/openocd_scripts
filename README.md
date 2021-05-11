# openocd scripts for JLINK or CMSIS-DAP

# Jlink script example
kenny@raspberrypi:~/scripts $ openocd -f mink_jlink.cfg 
Open On-Chip Debugger 0.10.0
Licensed under GNU GPL v2
For bug reports, read
	http://openocd.org/doc/doxygen/bugs.html
adapter speed: 2000 kHz
srst_only separate srst_gates_jtag srst_open_drain connect_deassert_srst
Info : No device selected, using first device.
Info : J-Link ARM V8 compiled May 27 2009 17:31:22
Info : Hardware version: 8.00
Info : VTarget = 3.345 V
Info : clock speed 2000 kHz
Info : JTAG tap: Mink.cpu tap/device found: 0x4ba00477 (mfg: 0x23b (ARM Ltd.), part: 0xba00, ver: 0x4)
Info : Mink.cpu: hardware has 6 breakpoints, 4 watchpoints


# CMSIS-DAP scritp example
kenny@raspberrypi:~/scripts $ openocd -f nrf52832_cmsis.cfg 
Open On-Chip Debugger 0.10.0
Licensed under GNU GPL v2
For bug reports, read
	http://openocd.org/doc/doxygen/bugs.html
adapter speed: 4000 kHz
srst_only separate srst_gates_jtag srst_open_drain connect_deassert_srst
Info : CMSIS-DAP: SWD  Supported
Info : CMSIS-DAP: Interface Initialised (SWD)
Info : CMSIS-DAP: FW Version = 1.10
Info : SWCLK/TCK = 1 SWDIO/TMS = 1 TDI = 0 TDO = 0 nTRST = 0 nRESET = 1
Info : CMSIS-DAP: Interface ready
Info : clock speed 4000 kHz
Info : SWD DPIDR 0x2ba01477
Info : NRF52832.cpu: hardware has 6 breakpoints, 4 watchpoints
