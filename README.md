pngpaste
========

Paste PNG into files, much like `pbpaste` does for text.

However instead of `pngpaste > thefile.png`, it's `pngpaste thefile.png`,
so one does not accidentally barf binary into the console.

You can also use the single character '-' instead of filename to redirect output to stdout (useful to pipe to other cli commands).

For example, to inverse image with ImageMagick :

    pngpaste - | convert -negate png:- inversed_image.png
    
### Motivation

[http://apple.stackexchange.com/q/11100/4795](http://apple.stackexchange.com/q/11100/4795)

### Build

    $ make all

### Installation

    $ sudo make install

### Usage

    $ pngpaste hooray.png

### Error Handling

Minimal :'(
