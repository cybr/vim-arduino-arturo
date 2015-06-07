# Vim Arduino Arturo

This script is a fork of [Vim Arduino Ino][vim-arduino-ino] and uses [Arturo][arturo] instead of [Ino][ino]. 
It runs in 64-bit environments and allows for compiling and
deployment of Arduino (\*.pde/\*.ino) sketches directly from Vim. It also allows the use of newer versions of the arduino IDE (1.6.1 at the current moment)

## Install
The easiest way to install this software is a plugin-manager like [Pathogen][pathogen] or [Vundle][vundle].

## Requirements
[Arturo][arturo] must be installed on your computer for this plugin to work.

## Usage
Vim Arduino Ino can be run using the following keys:

`<Leader>ac` - Compile the current sketch.

`<Leader>ad` - Compile and deploy the current sketch.

`<Leader>as` - Open a serial port in `screen`.

In order for the build to complete successfully, your project directory will need to be set up like a normal Arturo project.

## Options
The default key mapping can be turned off by doing this in your `.vimrc`:

```
let g:vim_arduino_map_keys = 0
```

To open the serial monitor automatically after each deploy,
add this to your `.vimrc`:

```
let g:vim_arduino_auto_open_serial = 1
```

[vim-arduino-ino]: https://github.com/jplaut/vim-arduino-ino/
[pathogen]: https://github.com/tpope/vim-pathogen
[arturo]: https://github.com/scottdarch/Arturo
[vundle]: https://github.com/gmarik/Vundle.vim
[ino]: http://inotool.org/
[arduino]: http://arduino.cc/en/Main/Software
[ino-project]: http://inotool.org/quickstart
