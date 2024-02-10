all:	result.vcd
result.vcd:	jk_flipflop.vhdl	jk_flipflop_test.vhdl
	ghdl	-a	-fsynopsys	jk_flipflop.vhdl
	ghdl	-a	-fsynopsys	jk_flipflop_test.vhdl
	ghdl	-e	-fsynopsys	testbench
	ghdl	-r	-fsynopsys	testbench	--vcd=result.vcd	--stop-time=20us
clean:
	rm	-rf	result.vcd