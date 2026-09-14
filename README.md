> **Note:** This is a slightly more modernized fork of the original `vscode-arm` extension by Mikhail Arkhipov. It fixes several formatting bugs regarding directives and comment alignments. 

# ARM Assembly Language support for Visual Studio Code
A [Visual Studio Code](https://code.visualstudio.com/) [extension](https://marketplace.visualstudio.com/items?itemName=omarorajain.arm-assembly-editor-modern) provides support for the [ARM Assembly language](https://developer.arm.com/documentation/dui0068/b/ARM-Instruction-Reference) when using GAS (GCC Assembler). 

![ARM Assembly editor](https://github.com/omarorajain/vscode-arm/blob/main/images/Screen1.png?raw=true)

# Features
Features include semantic coloring, tooltips/hover, completions, code formatting, basic syntax checking. Assembly syntax is [GAS/GCC](https://sourceware.org/binutils/docs/as/index.html#SEC_Contents)

## Colorizer
Adds new colorable items: 
- `directive` 
- `instruction`, 
- `register` 

and the following modifiers: 
- `definition` (symbols defined via `.set` or similar)
- `declaration` (data declarations such as `.asciz`).
- `include` (`.include` directive)
- `condition` (`.if/.endif/...` directives)
- `macro` (`.macro` directive)
- `macroName` (name of the macro)
- `macroParameter`, (macro parameter reference via `\\`)
- `unrecognized` (unrecognized instruction)

To customize colors combine item with modifiers, like `directive.include`.

## Hover
![ARM Assembly editor](https://github.com/omarorajain/vscode-arm/blob/main/images/Screen2.png?raw=true)

## Completions
![ARM Assembly editor](https://github.com/omarorajain/vscode-arm/blob/main/images/Screen4.png?raw=true)

## Instruction documentation in browser
![ARM Assembly editor](https://github.com/omarorajain/vscode-arm/blob/main/images/Screen3.png?raw=true)

## Formatting
Formatter by default automatically derives instruction set (architecture) as well as indentation and casing settings from the document. Options can be set to non-auto values in settings. 

## Limitations
- ARM Assembler syntax is not supported. 
- Syntax check is basic, the feature is far from complete and is diagnostics is off by default.
- Formatting does not support using tabs. Tabs are converted to spaces.