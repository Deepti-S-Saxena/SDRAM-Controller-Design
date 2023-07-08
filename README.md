**# SDRAM-Controller-Design**
The goal of this project is to design an SDRAM controller that allows SDRAM memory to be interfaced
with a microprocessor having only asynchronous memory support. There is no requirement to build the
hardware, but a complete written report containing schematics and theory of operation is required.

** Detailed Requirements
The SDRAM controller should be designed to interface with one or more SDRAM memory devices. The
minimum requirement is that support for a single MT48LC16M4A2 be provided. 

The detailed requirements follow:
1. Support the MT48LC16M4A2 memory device is required.
2. Support for a 80386DX or similar processor with 32-bit data bus not having SDRAM support is
required.
3. The use of “northbridge/MCH/IMCH” chipsets, SDRAM controller (including reference design or
commercial FPGA/CPLD/ASIC/hard copy solutions is not allowed).
4. A complete controller solution including state machine, row, column, and bank signal generation,
data masking, data flow, ready logic, and refresh support must be provided.
5. Interfacing with ~ADS, W/~R, and M/~IO control signals (or equivalent) will be required.
6. Support the sending of AUTO REFRESH commands at a rate sufficient to ensure memory
integrity.
7. Support the READY logic of the selected microprocessor system, especially when refresh is
occurring, unless a bus locking protocol is used.
8. Support is only required for burst length 8 transfers, although you may add different burst length
support for DMA operations if you wish for extra credit or support different bit-width memories
with different burst lengths as an option.
