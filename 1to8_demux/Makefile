all:	result.vcd
result.vcd:	1to8_demux.vhdl	1to8_demux_test.vhdl
	ghdl	-a	-fsynopsys	1to8_demux.vhdl
	ghdl	-a	-fsynopsys	1to8_demux_test.vhdl
	ghdl	-e	-fsynopsys	demux_test
	ghdl	-r	-fsynopsys	demux_test	--vcd=result.vcd
clean:
	rm	-rf	result.vcd
