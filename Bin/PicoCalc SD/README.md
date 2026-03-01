# PicoCalc SD v0.6
```
PicoCalc SD/
├── BellLabs_Fine.mp3
├── bifdiag.bas
├── BOOT2040.uf2
├── bootloader_pico.uf2
├── cc
│   ├── edit.lua
│   ├── expect.lua
│   ├── internal
│   │   ├── menu.lua
│   │   └── syntax
│   │       ├── errors.lua
│   │       ├── init.lua
│   │       ├── lexer.lua
│   │       └── parser.lua
│   └── pretty.lua
├── Chessnovice_johnybot.nes
├── fonts
│   ├── 6x10.fnt
│   ├── Acer8x8.fnt
│   ├── Haxor12.fnt
│   ├── HP6x8.fnt
│   ├── HP8x8.fnt
│   └── ProggyClean.fnt
├── lorenz.bas
├── lua
│   ├── asteroids.lua
│   ├── boxworld.bmp
│   ├── boxworld.lua
│   ├── browser.lua
│   ├── bubble.lua
│   ├── mandelbrot.lua
│   └── piano.lua
├── MACHIKAP.INI
├── main.lua
├── mand.bas
├── pico1-apps
│   ├── MicroPython_fa8b24c.uf2
│   ├── phyllosoma_kb.uf2
│   ├── PicoCalc_Fuzix_v1.0.uf2
│   ├── PicoCalc_MP3Player_v0.5.uf2
│   ├── PicoCalc_NES_v1.0.uf2
│   ├── PicoCalc_uLisp_v1.1.uf2
│   ├── picolua_daf20a2.uf2
│   ├── PicoMite_v6.02.01b4_beta.uf2
│   └── Picoware_v1.6.9.uf2
├── picocalc.bmp
├── picoware
│   ├── apps
│   │   ├── Calculator.mpy
│   │   ├── cat-fact.mpy
│   │   ├── counter.mpy
│   │   ├── flip_social
│   │   │   ├── __init__.py
│   │   │   ├── password.mpy
│   │   │   ├── run.mpy
│   │   │   ├── settings.mpy
│   │   │   └── username.mpy
│   │   ├── FlipSocial.mpy
│   │   ├── games
│   │   │   ├── 2048.mpy
│   │   │   ├── Breakout.mpy
│   │   │   ├── example.mpy
│   │   │   ├── Flappy Bird.mpy
│   │   │   ├── flip_world
│   │   │   │   ├── assets.mpy
│   │   │   │   ├── general.mpy
│   │   │   │   ├── __init__.py
│   │   │   │   ├── player.mpy
│   │   │   │   ├── run.mpy
│   │   │   │   └── sprite.mpy
│   │   │   ├── FlipWorld.mpy
│   │   │   ├── free_roam
│   │   │   │   ├── dynamic_map.mpy
│   │   │   │   ├── game.mpy
│   │   │   │   ├── __init__.py
│   │   │   │   ├── maps.mpy
│   │   │   │   ├── player.mpy
│   │   │   │   └── sprite.mpy
│   │   │   ├── Free Roam.mpy
│   │   │   ├── game_of_life.mpy
│   │   │   ├── Maze Runner.mpy
│   │   │   ├── Minesweeper.mpy
│   │   │   ├── Pong.mpy
│   │   │   ├── Snake.mpy
│   │   │   ├── Soduko.mpy
│   │   │   ├── Space Invaders.mpy
│   │   │   ├── Tetris.mpy
│   │   │   └── Tower Defense.mpy
│   │   ├── Graph.mpy
│   │   ├── hello_color.mpy
│   │   ├── keyboard-simple.mpy
│   │   ├── loading-simple.mpy
│   │   ├── menu-simple.mpy
│   │   ├── random-object.mpy
│   │   ├── screensavers
│   │   │   ├── Bubble Universe.mpy
│   │   │   ├── Clock.mpy
│   │   │   ├── Cube.mpy
│   │   │   ├── DVI Bounce.mpy
│   │   │   ├── Fire Effect.mpy
│   │   │   ├── Matrix Rain.mpy
│   │   │   ├── Patterns.mpy
│   │   │   ├── PicoFlower.mpy
│   │   │   ├── Plasma Wave.mpy
│   │   │   └── Yin-Yang.mpy
│   │   ├── Serial Terminal.mpy
│   │   ├── storage-simple.mpy
│   │   ├── textbox-simple.mpy
│   │   ├── Text Editor.mpy
│   │   └── Weather.mpy
│   └── settings
└── README.md

```

Since PicoCalc SD v0.6 we used [uf2loader](https://github.com/pelrun/uf2loader.git) as main loader.

All uf2 files in folder **pico1-apps** will be showed up in menu.

Once a uf2 got flashed and ran, next time you can use menu item **[Default App]** to directly run it without flashing it again.

Important files:  

* bootloader_pico.uf2   
  uf2loader main program, should be flashed into pico.
* BOOT2040.uf2   
  uf2loader Menu UI, it is a very important file, do not delete or edit it unless you know what you are doing.


## PicoCalc_Fuzix_v1.0.uf2  

[Fuzix](https://github.com/EtchedPixels/FUZIX.git) is an open-source, lightweight Unix-like operating system specifically designed for 8-bit and other resource-constrained processors.  

Patches for PicoCalc are [here](https://github.com/clockworkpi/PicoCalc/tree/master/Code/FUZIX)  
UF2 Path:   /pico1-apps/PicoCalc_Fuzix_v1.0.uf2 ([Download](https://github.com/clockworkpi/PicoCalc/tree/master/Bin/PicoCalc%20SD/pico1-apps))  

## pico1-apps/PicoCalc_NES_v1.0.uf2 

A simple NES emulator for PicoCalc, it will scan all nes files in the root of SD card.  
Given the resource constraints of the Pico, it is recommended to only run NES games that are less than **44KB** in size.

UF2 Path:  /pico1-apps/PicoCalc_NES_v1.0.uf2 ([Download](https://github.com/clockworkpi/PicoCalc/tree/master/Bin/PicoCalc%20SD/pico1-apps))  

## picolua_daf20a2.uf2  

https://github.com/Lana-chan/picocalc_lua  
A Lua interpreter for PicoCalc. It contains a REPL, basic API to draw graphics, read keys and access the SD filesystem.  

UF2 Path: /pico1-apps/picolua_daf20a2.uf2 ([Download](https://github.com/clockworkpi/PicoCalc/tree/master/Bin/PicoCalc%20SD/pico1-apps))   

## Picoware_v1.6.9.uf2  

https://github.com/jblanked/Picoware

An Open-source custom firmware for the PicoCalc, Video Game Module, and other Raspberry Pi Pico devices.  
 
Here is the version based on MicroPython.  

UF2 Path: /pico1-apps/Picoware_v1.6.9.uf2 ([Download](https://github.com/clockworkpi/PicoCalc/tree/master/Bin/PicoCalc%20SD/pico1-apps))    

## phyllosoma_kb.uf2   

[MachiKania Phyllosoma](https://github.com/machikania/phyllosoma/releases) is a BASIC compiler for ARMv6-M with excellent performance., especially for Raspberry Pi Pico.  

UF2 Path: /pico1-apps/phyllosoma_kb.uf2   ([Download](https://github.com/clockworkpi/PicoCalc/tree/master/Bin/PicoCalc%20SD/pico1-apps))   

## PicoCalc_MP3Player_v0.5.uf2

[PicoCalc_MP3Player](https://github.com/clockworkpi/PicoCalc/tree/master/Code/MP3Player)  is a simple MP3 playback program based on the [YAHAL](https://git.fh-aachen.de/Terstegge/YAHAL

) framework.

UF2 Path: /pico1-apps/PicoCalc_MP3Player_v0.5.uf2 ([Download](https://github.com/clockworkpi/PicoCalc/tree/master/Bin/PicoCalc%20SD/pico1-apps))    

## PicoCalc_uLisp_v1.1.uf2 

http://www.ulisp.com/show?56ZO

A self-contained Lisp computer for PicoCalc.   
UF2 Path: /pico1-apps/PicoCalc_uLisp_v1.1.uf2 ([Download](https://github.com/clockworkpi/PicoCalc/tree/master/Bin/PicoCalc%20SD/pico1-apps))   

## PicoMite_v6.02.01b4_beta.uf2  

[The PicoMite](https://geoffg.net/picomite.html) is a complete operating system with a Microsoft BASIC compatible interpreter and extensive hardware support including touch sensitive LCD panels, SD Cards, WiFi/Internet and much more.

UF2 Path: /pico1-apps/PicoMite_v6.02.01b4_beta.uf2 ([Download](https://github.com/clockworkpi/PicoCalc/tree/master/Bin/PicoCalc%20SD/pico1-apps))   

```
Copyright and Acknowledgments

The PicoMite firmware and MMBasic is copyright 2011-2025 by Geoff Graham and Peter Mather 2016-2025.
1-Wire Support is copyright 1999-2006 Dallas Semiconductor Corporation and 2012 Gerard Sexton.
FatFs (SD Card) driver is copyright 2014, ChaN.
WAV, MP3, and FLAC file support is copyright 2019 David Reid.
JPG support is thanks to Rich Geldreich
The pico-sdk is copyright 2021 Raspberry Pi (Trading) Ltd.
TinyUSB is copyright tinyusb.org
LittleFS is copyright Christopher Haster
Thomas Williams and Gerry Allardice for MMBasic enhancements
The VGA driver code was derived from work by Miroslav Nemecek
The CRC calculations are copyright Rob Tillaart
The compiled object code (the .uf2 file) for the PicoMite firmware is free software: you can use or redistribute
it as you please. The source code is on GitHub ( https://github.com/UKTailwind/PicoMiteAllVersions ) and
can be freely used subject to some conditions (see the header in the source files).
This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY, without even
the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```


##  MicroPython_fa8b24c.uf2  

https://github.com/zenodante/PicoCalc-micropython-driver

[MicroPython](https://micropython.org/) is a lean and efficient implementation of the Python 3 programming language that includes a small subset of the Python standard library and is optimised to run on microcontrollers and in constrained environments.

Here is the MicroPython Drivers compatible with PicoCalc.

UF2 Path: /pico1-apps/MicroPython_fa8b24c.uf2  ([Download](https://github.com/clockworkpi/PicoCalc/tree/master/Bin/PicoCalc%20SD/pico1-apps))   

