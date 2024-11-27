# ICS3203-CAT2-Assembly--Mwangi-Victor-Mbugu-151176

## Overview

This repository contains four assembly programs developed as part of the ICS3203 CAT 2 practical tasks. Each program is designed to demonstrate a specific set of skills related to assembly language programming. Below is a brief overview of each task and its purpose.

---

### Task 1: Control Flow and Conditional Logic

This program prompts the user to enter a number and classifies it as positive, negative, or zero. It demonstrates the use of jump instructions to manage control flow based on conditional checks.

#### Instructions:

1. **Compile using**:  
   ```bash
   nasm -f elf32 control_flow.asm -o control_flow.o
   ```

2. **Link using**:  
   ```bash
   ld -m elf_i386 control_flow.o -o control_flow
   ```

3. **Run using**:  
   ```bash
   ./control_flow
   ```

---

### Task 2: Array Manipulation with Looping and Reversal

This program accepts an array of five integers as input, reverses the array in place using loops, and outputs the reversed array. It avoids using additional memory for the reversed array, showcasing efficient use of looping constructs.

#### Instructions:

1. **Compile using**:  
   ```bash
   nasm -f elf32 array_reversal.asm -o array_reversal.o
   ```

2. **Link using**:  
   ```bash
   ld -m elf_i386 array_reversal.o -o array_reversal
   ```

3. **Run using**:  
   ```bash
   ./array_reversal
   ```

---

### Task 3: Modular Program with Subroutines for Factorial Calculation

This program calculates the factorial of a number between 1 and 10 using recursion. It includes modular subroutines and manages register values using the stack to preserve data during recursive calls.

#### Instructions:

1. **Compile using**:  
   ```bash
   nasm -f elf32 factorial_program.asm -o factorial_program.o
   ```

2. **Link using**:  
   ```bash
   ld -m elf_i386 factorial_program.o -o factorial_program
   ```

3. **Run using**:  
   ```bash
   ./factorial_program
   ```

---

### Task 4: Data Monitoring and Control Using Port-Based Simulation

This program simulates sensor input to control a motor and an alarm. It demonstrates decision-making based on sensor values and updates motor or alarm statuses by manipulating specific memory locations.

#### Instructions:

1. **Compile using**:  
   ```bash
   nasm -f elf32 port_simulation.asm -o port_simulation.o
   ```

2. **Link using**:  
   ```bash
   ld -m elf_i386 port_simulation.o -o port_simulation
   ```

3. **Run using**:  
   ```bash
   ./port_simulation
   ```

---

## Insights and Challenges

### Task 1

- **Insight**: Understanding control flow through jump instructions (`je`, `jl`, `jmp`) helped in clear classification logic.
- **Challenge**: Correctly converting ASCII input to integer while ensuring edge cases (like non-numeric input) are handled properly.

### Task 2

- **Insight**: Efficient in-place reversal minimizes memory usage and improves performance.
- **Challenge**: Managing loop counters and array boundaries required careful planning to prevent off-by-one errors.

### Task 3

- **Insight**: The modular design using subroutines made it easier to handle recursion and stack operations.
- **Challenge**: Ensuring proper preservation and restoration of register values during recursive calls was critical.

### Task 4

- **Insight**: Simulating real-time system control through memory manipulation provided practical insights into embedded systems.
- **Challenge**: Handling sensor value parsing and ensuring correct motor and alarm status updates.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
