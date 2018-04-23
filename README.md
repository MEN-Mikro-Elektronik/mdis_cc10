README for this MDIS project
----------------------------

CC10 default MDIS project for MDIS package 1.20 to test Z87/CAN behavior

this CC10 MDIS project contains driver Makefile for Z87 and MSCAN driver and fpga_load utility.

to build the drivers, either do a selfhosted build with a LSB root fs: install MDIS package and then just call make
or copy the modules to your CC10

Customerspecific FPGA table for this MDIS project:
Unit                devId   Grp Rev  Inst  IRQ   BAR  Offset      Addr
00 16Z024_SRAM      0x0018  0   14   0x00  0x3f   0   0x00000000  0x01110000
01 16Z127_GPIO      0x007f  0    8   0x00  0x03   0   0x00000100  0x01110100
02 16Z126_SERFLASH  0x007e  0   11   0x00  0x3f   0   0x00000200  0x01110200
03 16Z052_GIRQ      0x0034  0    5   0x00  0x3f   0   0x00000300  0x01110300
04 16Z087_ETH       0x0057  0   24   0x00  0x01   0   0x00000400  0x01110400
05 16Z087_ETH       0x0057  0   24   0x01  0x02   0   0x00000500  0x01110500
06 -CUSTOM-         0x0094  0    1   0x00  0x04   0   0x00000600  0x01110600
07 16Z029_CAN       0x001d  0   18   0x00  0x05   0   0x00000700  0x01110700
08 16Z029_CAN       0x001d  0   18   0x01  0x06   0   0x00000800  0x01110800
09 16Z127_GPIO      0x007f  0    8   0x01  0x07   0   0x00000a00  0x01110a00
10 16Z135_UART      0x0087  0   16   0x00  0x08   0   0x00001000  0x01111000
11 16Z135_UART      0x0087  0   16   0x01  0x09   0   0x00002000  0x01112000
12 -CUSTOM-         0x0095  1    0   0x00  0x00   0   0x00000900  0x01110900
13 16Z024_SRAM      0x0018  1   14   0x01  0x3f   1   0x00000000  0x01100000

