# Changelog

## 2026-03-04 (v3)

### Added
- Explanation Log — tabbed "Latest" / "Log" view, scrollable execution trace, Copy Log button, undo removes entries, reset clears log

## 2026-03-04 (v2)

### Added
- Stack memory change highlighting — recently written cells flash amber
- Register change highlighting — modified registers flash amber after each step
- Breakpoints — click the gutter dot on any executable line to set/clear; Run All stops at breakpoints
- Step Back / Undo — rewind one instruction at a time (up to 50 steps); Backspace keyboard shortcut
- Run speed slider — adjust execution interval from 50ms to 2000ms, live-updates during Run All
- Legend entries for changed-value highlight and breakpoint dot
- Keyboard shortcut reference in legend (Space, Backspace, Escape)

## 2026-03-04

### Added
- New instructions: TEST, SHL, SHR, NEG, XCHG
- Keyboard shortcuts: Space to step, Escape to stop Run All
- LEA instruction for address computation
- URL sharing — encode program in URL hash for easy sharing
- Next-instruction highlighting in the code editor

### Improved
- Updated supported instructions legend

## 2025-08-29

### Added
- Initial release of x86 Assembly Stack Simulator
- Instructions: PUSH, POP, MOV, ADD, SUB, XOR, AND, OR, NOT, INC, DEC, NOP, CMP, JMP, JZ/JE, JNZ/JNE, CALL, RET, ENTER, LEAVE
- Visual stack display with ESP/EBP highlighting
- Register panel with all general-purpose registers + EIP
- Zero flag tracking
- Step-through and Run All execution modes
- Inline explanations for each instruction
- Demo link in README

### Fixed
- Disabled auto-scrolling for smoother experience
