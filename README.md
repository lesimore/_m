# _m (in progress)
## A Language

`_m` (pronounced "underscum") is an esoteric interpreter language that simulates the **turing machine**. It's goal is to create a simple **turing complete** language that can be expanded to more complex structure.

There are 6 commands in `_m`. Here they are:

### Conditional commands:

`$` - this command details that the following function will only occur if the value of the current cell is *1*.

`#` - this command details that the following function will only occur if the value of the current cell is *0*.

### Movement commands:

`/` - this command moves the pointer to the right on the turing tape

`\` - this command moves the pointer to the left on the turing tape

### Value commands:

`!` - this command sets the value of a cell to *1*.

`x` - this command sets the value of a cell to *0*.

Each program has lines in it, and each line can contain a condition, movement, and/or value. The end of each line starts with either a %, for a line number to jump to, or a *, for a line name to jump to. Then, you can append the number or name. You can also name a line by appending a > to the end followed by the name.

The program that is provided in this repo can be imported in a C file to make an interface.
