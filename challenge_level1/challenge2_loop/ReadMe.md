BUG FOUND: 
Loop not exited 
![image](https://github.com/vyomasystems-lab/riscv-ctb-challenge-akshaya-2612/assets/102654877/eeb5ddb7-64b7-48ee-83e7-1fa8b8998483)

OBSERVATION: 
t5 register is initialized to 3, which indicated the total number of test cases.

FIXED:
1. Declared a register (t6) that is initialized to 0.
2. In the loop, if value at t6 != t3 then the loop is executed, otherwise loop is exited and branched to test_end
3. The value in t6 is incremented by 1 by using addi instruction.
![image](https://github.com/vyomasystems-lab/riscv-ctb-challenge-akshaya-2612/assets/102654877/8ed8289b-47ea-421f-ac6c-f3f362a7016b)


Successfully Run Test Case:
![image](https://github.com/vyomasystems-lab/riscv-ctb-challenge-akshaya-2612/assets/102654877/72044193-90b7-4398-bc8f-a5310f7c29dc)

