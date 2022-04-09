# CloverOS

Graphical Unix-like operating system for x86 computers.


## About

CloverOS is the mix of cool tools from other os shaped like unix core

Roughly speaking, the goal is a hybreed between the aesthetic of late-1990s productivity software and the power-user accessibility of late-2000s \*nix. This is a system by us, for us, based on the things we like.



**FAQ**: [Frequently Asked Questions](https://github.com/Dumbo-programmer/Clover-os/blob/master/Documentation/FAQ.md)

## Screenshot

![Screenshot as of b36968c.png](https://raw.githubusercontent.com/Dumbo-programmer/Clover-os/master/Meta/Screenshots/screenshot-b36968c.png)

## Features

* Modern x86 32-bit and 64-bit kernel with pre-emptive multi-threading
* [Browser](Userland/Applications/Browser/) with JavaScript, WebAssembly, and more (check the spec compliance for [JS](https://libjs.dev/test262/), [CSS](https://css.tobyase.de/), and [WASM](https://libjs.dev/wasm/))
* Security features (hardware protections, limited userland capabilities, W^X memory, `pledge` & `unveil`, (K)ASLR, OOM-resistance, web-content isolation, state-of-the-art TLS algorithms, ...)
* [System services](Userland/Services/) (WindowServer, LoginServer, AudioServer, WebServer, RequestServer, CrashServer, ...) and modern IPC
* Good POSIX compatibility ([LibC](Userland/Libraries/LibC/), Shell, syscalls, signals, pseudoterminals, filesystem notifications, standard Unix [utilities](Userland/Utilities/), ...)
* POSIX-like virtual file systems (/proc, /dev, /sys, /tmp, ...) and ext2 file system
* Network stack and applications with support for IPv4, TCP, UDP; DNS, HTTP, Gemini, IMAP, NTP
* Profiling, debugging and other development tools (Kernel-supported profiling, detailed program analysis with software emulation in UserspaceEmulator, CrashReporter, interactive GUI playground, HexEditor, HackStudio IDE for C++ and more)
* [Libraries](Userland/Libraries/) for everything from cryptography to OpenGL, audio, JavaScript, GUI, playing chess, ...
* Support for many common and uncommon file formats (PNG, JPEG, GIF, MP3, WAV, FLAC, ZIP, TAR, PDF, QOI, Gemini, ...)
* Unified style and design philosophy, flexible theming system, [custom (bitmap and vector) fonts](https://fonts.serenityos.net/font-family)
* [Games](Userland/Games/) (Solitaire, Minesweeper, 2048, chess, Conway's Game of Life, ...) and [demos](Userland/Demos/) (CatDog, Starfield, Eyes, mandelbrot set, WidgetGallery, ...)
* Every-day GUI programs and utilities (Spreadsheet with JavaScript, TextEditor, Terminal, PixelPaint, various multimedia viewers and players, Mail, Assistant, Calculator, ...)

... and all of the above are right in this repository, no extra dependencies, built from-scratch by us :^)

Additionally, there are [over two hundred ports of popular open-source software](Ports/AvailablePorts.md), including games, compilers, Unix tools, multimedia apps and more.

## How do I read the documentation?

When running you can use `man` for the terminal interface, or `help` for the GUI.

Code-related documentation can be found in the [documentation](Documentation/) folder.

## How do I build and run this?

See the [Clover OS build instructions](https://github.com/Dumbo-programmer/Clover-os/blob/master/Documentation/BuildInstructions.md). Serenity runs on Linux, macOS (aarch64 might be a challenge), Windows (with WSL2) and many other *Nixes with hardware or software virtualization.

## Get in touch and participate!

Before opening an issue, please see the issue policy
A general guide for contributing can be found in [`CONTRIBUTING.md`](CONTRIBUTING.md).

##Serenity Os Authors

* **Andreas Kling** - [awesomekling](https://twitter.com/awesomekling)
* **Robin Burchell** - [rburchell](https://github.com/rburchell)
* **Conrad Pankoff** - [deoxxa](https://github.com/deoxxa)
* **Sergey Bugaev** - [bugaevc](https://github.com/bugaevc)
* **Liav A** - [supercomputer7](https://github.com/supercomputer7)
* **Linus Groh** - [linusg](https://github.com/linusg)
* **Ali Mohammad Pur** - [alimpfard](https://github.com/alimpfard)
* **Shannon Booth** - [shannonbooth](https://github.com/shannonbooth)
* **Hüseyin ASLITÜRK** - [asliturk](https://github.com/asliturk)
* **Matthew Olsson** - [mattco98](https://github.com/mattco98)
* **Nico Weber** - [nico](https://github.com/nico)
* **Brian Gianforcaro** - [bgianfo](https://github.com/bgianfo)
* **Ben Wiederhake** - [BenWiederhake](https://github.com/BenWiederhake)
* **Tom** - [tomuta](https://github.com/tomuta)
* **Paul Scharnofske** - [asynts](https://github.com/asynts)
* **Itamar Shenhar** - [itamar8910](https://github.com/itamar8910)
* **Luke Wilde** - [Lubrsi](https://github.com/Lubrsi)
* **Brendan Coles** - [bcoles](https://github.com/bcoles)
* **Andrew Kaster** - [ADKaster](https://github.com/ADKaster)
* **thankyouverycool** - [thankyouverycool](https://github.com/thankyouverycool)
* **Idan Horowitz** - [IdanHo](https://github.com/IdanHo)
* **Gunnar Beutner** - [gunnarbeutner](https://github.com/gunnarbeutner)
* **Tim Flynn** - [trflynn89](https://github.com/trflynn89)
* **Jean-Baptiste Boric** - [boricj](https://github.com/boricj)
* **Stephan Unverwerth** - [sunverwerth](https://github.com/sunverwerth)
* **Max Wipfli** - [MaxWipfli](https://github.com/MaxWipfli)
* **Daniel Bertalan** - [BertalanD](https://github.com/BertalanD)
* **Jelle Raaijmakers** - [GMTA](https://github.com/GMTA)
* **Sam Atkins** - [AtkinsSJ](https://github.com/AtkinsSJ)
* **Tobias Christiansen** - [TobyAsE](https://github.com/TobyAsE)
* **Lenny Maiorani** - [ldm5180](https://github.com/ldm5180)
* **sin-ack** - [sin-ack](https://github.com/sin-ack)
* **Jesse Buhagiar** - [Quaker762](https://github.com/Quaker762)
* **Peter Elliott** - [Petelliott](https://github.com/Petelliott)
* **Karol Kosek** - [krkk](https://github.com/krkk)
* **Mustafa Quraish** - [mustafaquraish](https://github.com/mustafaquraish)
* **David Tuin** - [davidot](https://github.com/davidot)
* **Leon Albrecht** - [Hendiadyoin1](https://github.com/Hendiadyoin1)
* **Tim Schumacher** - [timschumi](https://github.com/timschumi)
* **Marcus Nilsson** - [metmo](https://github.com/metmo)
* **Gegga Thor** - [Xexxa](https://github.com/Xexxa)
* **kleines Filmröllchen** - [kleinesfilmroellchen](https://github.com/kleinesfilmroellchen)
* **Kenneth Myhra** - [kennethmyhra](https://github.com/kennethmyhra)
* **Maciej** - [sppmacd](https://github.com/sppmacd)
* **Sahan Fernando** - [ccapitalK](https://github.com/ccapitalK)


## License

SerenityOS was licensed under a 2-clause BSD license.
