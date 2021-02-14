---
Title: Getting started
Description: The z80 development kit
---

## Getting started

Assuming you want to compile for a supported target, and with
over 100 targets to choose from, the chances are you are! Then it's easy to
produce an "executable" with z88dk, it's just a single command. Let's create a .TAP file for use with ZX Spectrum emulators:

```
zcc +zx program.c -create-app
```

How about a bootable +3 Spectrum disc?

```
zcc +zx program.c -create-app -subtype=plus3
```

Need it for CP/M instead? Try this:

```
zcc +cpm program.c -create-app
```

And a `.com` file is created. Do you want to test the `.com` file using
z80pack? It's much easier to test with a disc image, so let us create one:

```
zcc +cpm program.c -create-app -subtype=z80pack
```

Oh, it's an 8080 CP/M machine you're targetting, of course:

```
zcc +cpm -clib=8080 program.c -create-app -subtype=z80pack
```

An 8080 CP/M machine with a Polymorphic VTI graphics card?

```
zcc +cpm -clib=8080 program.c -create-app -subtype=z80pack --vti
```

## z88dk is the easiest way to use sdcc for z80

Seriously it really is, lets do it:

```
zcc +cpm program.c -create-app -subtype=z80pack -compiler=sdcc
```

Easy as that, no messing around with crt files, linker scripts,
hex2bin, cpmtools etc, just one command producing a disk image containing
a binary compiled with sdcc.
