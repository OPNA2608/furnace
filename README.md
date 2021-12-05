# Furnace

this is a work-in-progress chip music player (currently) for the .dmf format.

## features

- supports Sega Genesis, Master System, Game Boy, PC Engine, NES and C64 (for now, with more systems coming soon)
- clean-room design (zero reverse-engineered code and zero decompilation; using official DMF specs, guesswork and ABX tests only)
- bug/quirk implementation for increased playback accuracy
- accurate emulation cores (Nuked, MAME, SameBoy, Mednafen PCE, puNES and reSID (hahaha!))
- open-source. GPLv2.

## dependencies

- CMake
- SDL2
- zlib
- JACK (optional)

SDL2 and zlib are included as submodules for Windows and macOS.

## compilation

your typical CMake project. clone (including submodules) and:

### Windows using MSVC

from the developer tools command prompt:

```
mkdir build
cd build
cmake ..
msbuild ALL_BUILD.vcxproj
```

### macOS and Linux

```
mkdir build
cd build
cmake ..
make
```

## usage

```
./furnace <file>
```

this will play a file (must be in .dmf format).
