---
Title: Home
Description: The z80 development kit
---

# What is z88dk?

z88dk is the only C and assembler development kit that 
comes ready out-of-the-box to create programs for over
100 z80-family machines.

The project was started in 1998/9 to allow a TCP stack
for the Cambridge z88 to be easily written. In recent years
significant work has been undertaken to improve the number
of targets supported, enhance library features, make the
toolchain easier to use and improve life for developers.

## z88dk is dedicated to z80 family machines

Because we only target z80 family machines we can create optimised libraries. When you use z88dk, you
automatically use a C standard library that is mostly written in assembler.

The [library](https://github.com/z88dk/z88dk/tree/master/libsrc) consists
of over 15000 files containing at least 250k lines of assembler code. It's
probably the largest repository of z80 assembler source code online.

## z88dk is flexible

The point of any development kit should be to make life easy for you, the developer, and allow you to focus on writing your
application and not on figuring out how to turn a hex file
into a loadable artefact. As a result, the default setup for z88dk
is [configured](gettingstarted) to just make things work.

However, we know developers love twiddling knobs, after all, we're developers 
too. So with z88dk you can tune sizes, toggle
features on and off, choose different floating point libraries, switch library implementations, override
library implementations, bypass crts, turn off using the standard library. 

And yes, you can even generate hex files should you wish!




