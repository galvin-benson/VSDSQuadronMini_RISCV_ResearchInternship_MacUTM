# VSDSQuadronMini_RISCV_ResearchInternship_MacUTM
<details>
  <summary><big><b>Click Me😊</b></big></summary>
  <p>Hiii! I'm Galvin Benson<br>Email ID: galvin.benson@gmail.com<br>GitHub Profile: https://github.com/galvin-benson<br>LinkedIn Profile: www.linkedin.com/in/galvin-benson

</p>
</details>


A practical internship focused on RISC-V development using the VSDSQuadron Mini, covering setup, instruction analysis, simulation, and real-world embedded system applications.
All on a MacBook running Ubuntu via UTM!
![image](https://github.com/user-attachments/assets/0f0091ae-8a07-4903-ac24-8c1342084913)
<details>
<summary><big><b>TASK-1: </b></big>The objective of this task is to set up the necessary software environment for the internship. This includes installing Ubuntu on Mac UTM configuring the given riscv-toolchain-rv32imac-aarch64, and writing a simple C program. Additionally, the task involves evaluating the corresponding RISC-V assembly code generated from the sample C code. </summary>
<img width="810" alt="Screenshot 2025-02-26 at 11 37 34 PM" src="https://github.com/user-attachments/assets/7d60cb73-01ef-47b8-affe-5ab86f572497" />
<h3>Step:1 Setup of RISCV toolchain</h3>
<p>Extract the toolchain</p>
  
![image](https://github.com/user-attachments/assets/ce30157a-4a39-4574-80df-b674314f8d67)

![image](https://github.com/user-attachments/assets/5a7f5595-db06-48ae-bce2-1955123ab8f4)

<p>Add the path</p>

```plaintext
$ echo 'export PATH=/opt/riscv/bin:$PATH' >> ~/.zshrc
$ source ~/.zshrc
```

![image](https://github.com/user-attachments/assets/ffad5d86-e5ed-4280-9c62-d651ac65d3e5)


<h3>Step:2 Create a sample C code</h3>

<p>Create a new C file and write a basic code for compilation</p>

```plaintext
$ nano sum1ton.c
```

![image](https://github.com/user-attachments/assets/a29ef179-5705-4f01-8106-2c5dfc13aefd)


<h3>Step:3 Compile the C Code with basic GCC Compiler</h3>
<p>After writing a basic C code, compile the C code</p>

```plaintext
$ gcc sum1ton.c
```

<p>Now, Run the compiled C code</p>

```plaintext
$ ./a.out
```

![image](https://github.com/user-attachments/assets/51b2a9f7-f643-41ee-ba8a-89916f620096)

<h3>Step:4 Compile the C Code with RISC-V Compiler</h3>
<p>Compilation of the C code using RISC-V compiler:</p>

```plaintext
$ riscv32-unknown-elf-gcc -o hello_riscv.elf hello.c
$ spike --isa=rv32imac /opt/riscv/riscv32-unknown-elf/bin/pk  sum1ton_riscv.elf
```

![image](https://github.com/user-attachments/assets/d51ef008-a2ee-40a4-8fce-1bc9b1b25ac7)

<h3>Step 5: Display The Assembly Code</h3>
<p>To Display the optimized assembly code for the main function:</p>

```plaintext
$ riscv32-unknown-elf-objdump -d -S sum1ton_riscv.elf | less
```

![image](https://github.com/user-attachments/assets/7ead31ba-49a7-48aa-a415-26a54e1d9c6d)

</details>
