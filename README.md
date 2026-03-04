# x86 Assembly Stack Simulator

An interactive web-based simulator for visualizing how x86 assembly instructions affect the CPU registers and stack memory. This educational tool helps students and developers understand low-level programming concepts by providing real-time visualization of stack operations.

## Demo

Check out the demo at [https://wellingtonlee.github.io/stack-simulator/](https://wellingtonlee.github.io/stack-simulator/)

## Features

- **Interactive Code Editor**: Write and edit x86 assembly code directly in the browser
- **Step-by-Step Execution**: Execute instructions one at a time to see their effects
- **Real-Time Visualization**: Watch how the stack grows and shrinks with each instruction
- **Register Monitoring**: View current values of all CPU registers (EAX, EBX, ECX, EDX, ESP, EBP, EIP)
- **Stack Memory View**: Visual representation of stack memory with ESP and EBP highlighting
- **Detailed Explanations**: Get explanations for each instruction as it executes
- **Execution Log**: Browse full explanation history in the "Log" tab, copy execution trace to clipboard

## How to Use

1. **Open the Simulator**: Open `index.html` in any modern web browser
2. **Edit Assembly Code**: The left panel contains an editable code area with example assembly code
3. **Execute Instructions**: Click "Execute Next" to step through instructions one by one
4. **Monitor Changes**: Watch the registers and stack memory update in real-time
5. **Reset**: Click "Reset" to return to the initial state and try different code

## Supported Instructions

- **PUSH** - Push value onto stack
- **POP** - Pop value from stack into register
- **MOV** - Move data between registers and memory
- **ADD** - Add values to registers
- **SUB** - Subtract values from registers
- **CALL** - Call function (pushes return address)
- **RET** - Return from function (pops return address)
- **ENTER** - Function prologue (push EBP, set EBP to ESP)
- **LEAVE** - Function epilogue (restore ESP and EBP)

## Operand Types

- **Registers**: EAX, EBX, ECX, EDX, ESP, EBP
- **Immediate Values**: Decimal numbers (e.g., 10, 42)
- **Memory Access**: `[esp+offset]` or `[ebp-offset]` syntax
- **Labels**: For function calls and jumps

## Visual Legend

- **Blue highlight**: ESP (Stack Pointer) position and current executing line
- **Red highlight**: EBP (Base Pointer) position
- **Stack grows downward**: Higher addresses at top, lower addresses at bottom

## Educational Use

This simulator is perfect for:
- Learning x86 assembly language basics
- Understanding stack frame operations
- Visualizing function calls and returns
- Debugging stack-related issues
- Teaching low-level programming concepts

## Example Code

The simulator comes with example code that demonstrates:
- Basic register operations
- Stack manipulation with PUSH/POP
- Memory access using stack pointers
- Function calls with stack frame setup
- Local variable allocation

Simply click "Execute Next" repeatedly to see how each instruction affects the system state.

## Vibe Code Prompts

Coded with ❤️ using Gemini 2.5 Pro and the below prompts.

> A single page local webapp that helps explain the stack in x86 assembly when instructions are executed and how the stack changes with certain x86 assembly instructions like pop and push.

> This looks great. Can you make it so that the assembly code is side by side with the stack memory and registers in a more readable way?

> Add a highlight or indicator to show what line of assembly is about to be executed.