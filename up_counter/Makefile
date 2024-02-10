
all:	result.vcd
result.vcd:	up_counter.vhdl	up_counter_test.vhdl
	ghdl	-a	-fsynopsys	up_counter.vhdl
	ghdl	-a	-fsynopsys	up_counter_test.vhdl
	ghdl	-e	-fsynopsys testbench
	ghdl	-r	-fsynopsys testbench	--vcd=result.vcd	--stop-time=20us
clean:
	rm	-rf	result.vcd