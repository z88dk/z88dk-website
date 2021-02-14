---
Title: Getting started
Description: The z80 development kit
---

## Getting started

Assuming you want to compile for a supported target, and with
over 100 targets chances are you are! Then it's easy to
produce an "executable" with z88dk, it's just a single command. Let's create a .TAP file for use with ZX Spectrum emulators:

```
zcc +zx program.c -create-app
```

Need it for CP/M? Try this:

```
zcc +cpm program.c -create-app
```

And a `.com` file is created. Do you want to test the `.com` file using
z80pack? It's much easier to test with a disk image, so lets create one:

```
zcc +cpm program.c -create-app -subtype=z80pack
```

Oh, it's an 8080 machine you're targetting, of course:

```
zcc +cpm -clib=8080 program.c -create-app -subtype=z80pack
```

## z88dk is the easiest way to use sdcc for z80

Seriously it really is, lets do it:

```
zcc +cpm program.c -create-app -subtype=z80pack -compiler=sdcc
```

Easy as that, no messing around with crt files, linker scripts,
hex2bin, cpmtools etc, just one command producing a disk image containing
a binary compiled with sdcc.
