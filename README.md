# ZFMT - Drop in, customizable, unofficial zig formatter.

## Versioning
Zfmt uses zig 0.15.1, and its formatter is based off of zig fmt version 0.15.1

Zfmt will be usable with all modern zig versions.

## Options
### indent_delta = 4
indentation amount

### .asm_indent_delta = 4,
inlined assembly indentation amount

### .brace_style = .k_and_r,
brace style

available options:
1. k_and_r
```zig
fn main() void {
  // hello world
}
```
2. allman
```zig
fn main() void 
{
  // hello world
}
```

Note that allman style can break pre-existing code.

### .space_around_ops = true,

true: `1 + 2`

false: `1+2`

## Bugs
I made this formatter in less than a day (12 hours or so)

so there is probably some issues, if you encounter any then make an issue or a pull request.

## Why make this/"Consistency matters more! zig fmt was made so we have 1 coding style!"
I fundamentally disagree with that idea.

Tool inflexibility often breaks off ecosystems more than unify together, zfmt is a prime example of that.

I myself before making zfmt forked the entire zig compiler just to get 8 space indentation

I think that the fact zig is so opinionated is its biggest flaw.

If you disagree, then just use the opinionated zig fmt.
