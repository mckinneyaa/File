# File
A small class for making it a little easier to load files using either SDL_RWops or stdio.h functionallity. It is cross platform
and ready to go. I have only test on linux thus far, but will be building on windows soon.

##Origin
This class came about while learning about game engine development and I decided I wanted to use it in my petcode projects lexer.
It continues to gain new features and functionality.

##Building
This library does not require to be built it is now a header only library. If you wish to use the SDL_RWops.h functionality.
You will have to link with the SDL2 library otherwise it requires no library links other than the standard c library.

Then to build the test file perform the following
```bash
g++ src/test/teststdio.cpp -o test -I./include
g++ src/test/testsdl.cpp -o testsdl -I./include -lSDL2
```
Note: these instructions are for the main repository directory.

##Usage
when you include the file to use the SDL system you need to define FILE_SDL
```c++
#define FILE_SDL
#include "File.hpp"
```
For more information on usage see the documentation page https://github.com/mckinneyaa/File/wiki/Documentation

##TO-DO
* ~~convert the comments into documentation~~
* ~~make it a header only library~~
* add more features and functionality


####Licesne
MIT License

Copyright (c) 2016 Aaron McKinney

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
