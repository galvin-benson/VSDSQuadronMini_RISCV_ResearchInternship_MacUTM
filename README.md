# VSDSQuadronMini_RISCV_ResearchInternship_MacUTM
<details>
  <summary><big><b>Click Me😊</b></big></summary>
  <p>Hiii! I'm Galvin Benson<br>Email ID: galvin.benson@gmail.com<br>GitHub Profile: https://github.com/galvin-benson<br>LinkedIn Profile: www.linkedin.com/in/galvin-benson

</p>
</details>


A practical internship focused on RISC-V development using the VSDSQuadron Mini, covering setup, instruction analysis, simulation, and real-world embedded system applications.

![image](https://github.com/user-attachments/assets/0f0091ae-8a07-4903-ac24-8c1342084913)
<details>
<summary><big><b>TASK-1 : </b></big>The objective of this task is to set up the necessary software environment for the internship. This includes installing Ubuntu on VirtualBox, configuring Visual C++, and writing a simple C program. Additionally, the task involves evaluating the corresponding RISC-V assembly code generated from the sample C code. </summary>
<img width="810" alt="Screenshot 2025-02-26 at 11 37 34 PM" src="https://github.com/user-attachments/assets/7d60cb73-01ef-47b8-affe-5ab86f572497" />
<h3>Step:1 </h3>

```plaintext

```

<h3>Step:2 Create a sample C code</h3>
<p>Install Leafpad, a lightweight text editor for Ubuntu.</p>

```plaintext
  $ sudo apt install leafpad
```

<p>Create a new C file and write a basic code for compilation</p>

```plaintext
  $ leafpad sum1ton.c &
```

<img src="https://github.com/user-attachments/assets/ac56230c-35b3-4806-96ba-c1bcc3f5df43" alt="Screenshot" width="500">

<h3>Step:3 Compile the C Code with basic GCC Compiler</h3>
<p>After writing a basic C code, compile the C code</p>

```plaintext
  $ gcc sum1ton.c
```

<p>Now, Run the compiled C code</p>

```plaintext
  $ ./a.out
```

![Screenshot from 2025-02-26 22-50-14](https://github.com/user-attachments/assets/56c1a1a2-d30f-4532-985b-27f0564ee73a)
<br>Changing n value from 5 to 11.

![Screenshot from 2025-02-26 22-52-06](https://github.com/user-attachments/assets/0d1b8b10-cfed-47b9-b46b-86d8664dbe59)
![Screenshot from 2025-02-26 22-52-14](https://github.com/user-attachments/assets/16af63d5-d927-4962-b2f7-523f316783d5)


<h3>Compile the C Code with RISC-V Compiler</h3>
<p>Compilation of the C code using RISC-V compiler:</p>

```plaintext
  $ riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
```

![Screenshot from 2025-02-26 23-09-40](https://github.com/user-attachments/assets/2aac33a7-a85b-48dd-bcc1-67974f08473c)

<h3>Step 5: Display The Assembly Code</h3>
<p>To Display the optimized assembly code for the main function:</p>

```plaintext
  $ riscv64-unknown-elf-objdump -d filename.o | less
```

![Screenshot from 2025-02-26 23-09-27](https://github.com/user-attachments/assets/7cf6ef8d-ecfb-4ff9-bb4a-16fc84fa8a0d)

</details>
