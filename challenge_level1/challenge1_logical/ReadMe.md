**BUGS FOUND:** 

![image](https://github.com/vyomasystems-lab/riscv-ctb-challenge-akshaya-2612/assets/102654877/d6e99be3-77b7-4f56-ab97-7137aec86369)

**BUG 1:  Illegal Operands**
* The register z4 is not defined in RISC-V ISA. Therefore, it's invalid.
* It is fixed by replacing z4 with s4 because s4 is defined in the RISC-V ISA.
  
![image](https://github.com/vyomasystems-lab/riscv-ctb-challenge-akshaya-2612/assets/102654877/4017fd29-3bb1-4fea-9c62-2b7d32a0f9ff)

 
**BUG 2: Illegal Operands**
* The andi (and immediate) instruction requires the third operand to be an immediate value.
* Here, the third operand is a register (s0) which is not immediate. Therefore, it's invalid.
* It is fixed by replacing s0 by an immediate value 3
  
![image](https://github.com/vyomasystems-lab/riscv-ctb-challenge-akshaya-2612/assets/102654877/60f9072f-3583-4936-b1f5-27aeb5350521)

