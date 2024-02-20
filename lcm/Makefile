all:	result.vcd
result.vcd:	lcm.vhdl	lcm_test.vhdl
	ghdl	-a	-fsynopsys	lcm.vhdl
	ghdl	-a	lcm_test.vhdl
	ghdl	-e	-fsynopsys fsmtb_lcm
	ghdl	-r	-fsynopsys fsmtb_lcm	--vcd=result.vcd	--stop-time=20us
clean:
	rm	-rf	result.vcd