---
Title: Home
Description: The z80 development kit
---

# What is z88dk?

z88dk is the only C and assembler development kit that allows the 
creation of programs for over 100 z80-family machines. 

The project was started in 1998/9 to allow a TCP stack
for the Cambridge z88 to be easily written. In recent years
significant work has been undertaken to improve the number
of targets supported, enhance library features, make the
toolchain easier to use and improve life for developers.

## z88dk is dedicated to z80 family machines

Because we only target z80 family machines we can optimise! That
means the core performance sensitive parts of the C standard
library are written in 100% assembler.

The [library](https://github.com/z88dk/z88dk/tree/master/libsrc) consists
of over 15000 files containing at least 250k lines of assembler code. It's
probably the largest repository of z80 assembler source code online.

## z88dk is flexible

The point of any development kit should be to make life easy for you
as the developer and allow you to focus on writing your
application and not on figuring out how to turn a hex file
into a loadable artefact. As a result, the default setup for z88dk
is [configured](gettingstarted) to just make things work.

However, we know developers love twiddling knobs, we're developers 
too after all, so with z88dk you can tune sizes of things, toggle
features on and off, switch library implementations, override
library implementations, bypass crts, turn off using the standard
library. And yes, generate hex files should you wish!


