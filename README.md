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

Each program is built up of **pages**, which are each individual files. Each **page** can have at most one conditional, one movement, and one value command. At the end of a file, there is a filename enclosed in two *|*s.

Now, you may be wondering how you can get input, or how you can output information, and the answer is complicated. To input information, you have to make a seires of input pages that input data into some cells. The solution of the next problem is integrated into the interpreter. At the end of a program, the values of each cell are printed out. To output characters, you simply have to encode them into binary, and then have the user of your program decode them.
