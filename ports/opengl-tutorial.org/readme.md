# D2 Port of opengl-tutorial.org

The [opengl-tutorial.org] project is a set of C++ tutorials covering OpenGL v3.3+.

The included D [port][opengl-tutorial-port] contains all of the code samples which have been ported into D.

[opengl-tutorial.org]: http://www.opengl-tutorial.org/
[opengl-tutorial-port]: https://github.com/AndrejMitrovic/opengl-tutorials/tree/master/ports/opengl-tutorial.org

## Requirements

You will need to install the [glfw] shared library.
Make sure it's in your `PATH` environment variable,
or alternatively copy the [glfw] shared library to the `bin`
folder where the samples are built.

## Building the samples

All of the samples in this repository can be built using [dub]:

```
# note: In an upcoming dub release this will be 'dub run :tut01'
$ dub run opengl-tutorial.org:tut01

# alternatively
$ cd code/tut01
$ dub
```

## Tutorial Reading Guide

Since this is a D port many things can be ignored in the original tutorial.
You won't have to worry about setting up a build environment or have to manually
install dependencies. Simply use [dub] to build and run any sample.

The following is a list of chapter-specific guides for D developers.

### Tutorial 1 : Opening a window

Tutorial link:
http://www.opengl-tutorial.org/beginners-tutorials/tutorial-1-opening-a-window/

This chapter can largely be ignored, you won't have to set up a complex build environment.

Note about GLEW: This library isn't used, instead we're using [glad] to load all OpenGL function pointers,
including any extensions.

## License

Unless noted otherwise, samples are distributed under the [WTFPL Public License][WTFPL_License], Version 2, December 2004.

[dub]: http://code.dlang.org/download
[WTFPL_License]: http://www.wtfpl.net/txt/copying
[glad]: https://github.com/Dav1dde/glad