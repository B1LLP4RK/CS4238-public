# GCC cheatsheet for reverse engineering

- `help`
  - please read it, essential as a starting point
  - use `help command` for any command help messages
- `x`
  - must see help file for helpful options with `help x`
  - can use function names with * like `*main+1`
  - continuously press enter to see consecutive memory addresses
  - can access registers with `x $rbp`

- `print`
  - similar but serves different purpose than `x`
  - can see addresses of variables

- `layout asm`
  - shows assembly code with the CLI
  - if it doesn't show assembly, use `layout prev`, `layout next`
  - use  `C-x a` to toggle between layout mode and cli mode
  - in layout mode, use arrow keys to scroll through assembly code

- `info`
  - shows help messages

- `run`
- `continue`
- `info b`
  - based on the branch numbers, to `disable number` or `enable number`
- `info locals`
  - shows local variables
- `next`
  - executes next line of c code
- `ni`
  - executes next line of assembly code
- `step`
  - step into the function

> [!IMPORTANT]
> At certain point, the python package pwntools is required for
> feeding in non-ascii bytes to executable binaries. For more information
> go to [CTF-haven](https://github.com/B1LLP4RK/CTF-haven.git) 
