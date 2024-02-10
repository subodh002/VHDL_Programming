all:	result.vcd

result.vcd:	2to4_decoder.vhdl	2to4_decoder_test.vhdl
	ghdl	-a	-fsynopsys	2to4_decoder.vhdl
	ghdl	-a	-fsynopsys	2to4_decoder_test.vhdl
	ghdl	-e	-fsynopsys	testbench
	ghdl	-r	-fsynopsys	testbench	--vcd=result.vcd
clean:
	rm	-rf	result.vcd