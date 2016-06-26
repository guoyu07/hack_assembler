# hack_assembler

An implementation of the assembler for the Hack computer, described on
[Chapter 6][0] of ["From NAND to Tetris"][1] course.

## Installation

    $ pip install hack_assembler

## Usage

Consider the following file `Add.asm`:

    // This file is part of www.nand2tetris.org
    // and the book "The Elements of Computing Systems"
    // by Nisan and Schocken, MIT Press.
    // File name: projects/06/add/Add.asm
    
    // Computes R0 = 2 + 3
    
    @2
    D=A
    @3
    D=D+A
    @0
    M=D

Invoke the `hack-assembler` binary passing the file:

    $ hack-assembler Add.asm
    0000000000000010
    1110110000010000
    0000000000000011
    1110000010010000
    0000000000000000
    1110001100001000

## License

[Apache License 2.0][2].

[0]: http://nand2tetris.org/06.php
[1]: http://nand2tetris.org
[2]: https://github.com/thiagoalessio/hack_assembler/blob/master/LICENSE