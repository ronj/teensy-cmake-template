# teensy-cmake-template
CMake template for use with the Teensy Arduino compatible development board from PJRC (https://www.pjrc.com/teensy/index.html)

Using the template
==================

This CMake template for Teensy builds a blinking led example.

Prerequisites
-------------

Install Arduino IDE and Teensyduino according to [PJRCs guide](https://www.pjrc.com/teensy/td_download.html).


Build
-----

cd teensy-cmake-template
mkdir build
cmake .. -DCMAKE_TOOLCHAIN_FILE=toolchains/teensy.cmake
make


Build output
------------

Running the above commands will create a ELF file and a HEX file. The HEX file is automatically loaded in the Teensy loader application.


TODO
----

- Add add_library macro.
- Remove warnings when compiling C files. C file compilation is done with CPP flags, they are ignored but a warning is given. Is there a way to add_target_properties for C and CPP compilation separately?
- Check on more platforms than OSX.
