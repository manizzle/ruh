Ruh

Higher level goal: Audit code minimization
Sometimes you do not need all the code in the code base to figure out what are the relevant components to what you are looking for. This makes manual source code auditing much easier.

Say you have a program that has authentication. You want to be able to find which code paths are traversed when certain data is accessed. Just doing diffs of code coverage is difficult because the data that is parsed is not always an optional field(headers) and so you cannot just remove the data and watch it change paths. Sometimes it is blocking to the program. Authentication, headers, file container parsers are all ripe for this kind of work. DWARF, ELF, MachO, 

Create a system by which taint analysis finds code blocks that contain custom tainted variables. These code blocks are then marked back in the source code and functions can be parsed out.

1. Tools:
    1. Triton
2. Methodologies
    1. Taint Analysis
3. Previous Work
    1. DWARF debug info

