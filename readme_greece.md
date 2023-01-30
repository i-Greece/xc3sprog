# add nanoflow (ft2232h b) to cablelist.txt
	nanoflow      ftdi   30000000 0x0403:0x6010:Digilent Adept USB Device B:1   

# check jtag chain
	xc3sprog -c nanoflow -L -j -v

# program bitstream
	xc3sprog -L -v -c nanoflow led.bit
	xc3sprog -L -v -c nanoflow D:\Project\C++\xc3sprog\fpga\led.bit
	
# program flash
	
