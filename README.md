# _m
## A Language

`_m` is an esoteric interpreter language that simulates the **turing machine**. It's goal is to minimize the size of an interpreter while still being **turing complete**.

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

Each program is built up of **pages**, which are each individual files. Each **page** can have at most one conditional, one movement, and one value command. At the end of a file, there is a filename enclosed in two |s.
