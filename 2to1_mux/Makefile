all: result.vcd
result.vcd:	2to1_mux.vhdl	2to1_mux_test.vhdl
	ghdl	-a	-fsynopsys	2to1_mux.vhdl
	ghdl	-a	-fsynopsys	2to1_mux_test.vhdl
	ghdl	-e	-fsynopsys	testbench
	ghdl	-r	-fsynopsys	testbench	--vcd=result.vcd	--stop-time=20us
clean:
	rm	-rf	result.vcd