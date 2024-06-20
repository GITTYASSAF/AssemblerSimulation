## Assembler
project goal is to translate assembly files to binary files which are used by the linker program for assembly.

### Input files
Source file of instructions with extension ".as", for example ps.as.

### Output files
There are at most 4 output files:

".am" file of instructions after expanding macro statements.
".ob" file containing the machine code.
".ext" external label codes produce only if their is an external label .
".ent" entries label codes produce only if their is an entries label.
### More details about running
Program can receive multiple ".as" files as an input, but will refer to each file separately. If there is error in line of instruction, program will print error type into terminal and continue execution. Line that contains an error will be ignored in further steps.

### Running steps
- Preprocessor:

  Receives ".as" file and creates ".am" after expanding macro statements.

- First step:

  Get the file that the user enter and read it, while reading the function counter how many place the file need for the data and for the commands.

- Second step:

  parse the first time the file, and encode the file according to the commands or directive, that is writen in the file, the function cautions if an input error exists. Third step:

  Keep track of location counter, translate instructions and output into files.
