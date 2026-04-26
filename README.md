# Project README

## Overview
The project is a simple 2D physics simulation using the SAT (Separating Axis Theorem) algorithm. It provides a basic framework for creating and rendering 2D convex polygons, checking their collisions, and displaying them on a window.

## Features
- Creation and manipulation of 2D convex polygons.
- Collision detection using the SAT algorithm.
- Rendering of polygons with different colors based on selection.
- Support for multiple platforms:
  - Linux
  - Windows
  - Web (using Emscripten)
  - Wine (for cross-compiling to Windows)

## Project Structure
### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools
- Libraries needed in specific projects:
  - Linux: X11, pthreads
  - Windows: WINAPI
  - Web: Emscripten
  - Wine: Mingw-w64

## Build & Run
### Linux
To build and run on Linux:
```sh
cd <Project>
make -f Makefile.linux all
make -f Makefile.linux exe
```

### Windows
To build and run on Windows:
```sh
cd <Project>
make -f Makefile.windows all
make -f Makefile.windows exe
```

### Web
To build and run the project for web (using Emscripten):
```sh
cd <Project>
make -f Makefile.web all
emrun --no_browser --port 8080 ./build
```

### Wine
To build and run on Windows using Wine:
```sh
cd <Project>
make -f Makefile.wine all
make -f Makefile.wine exe
```

These instructions provide a straightforward way to set up, compile, and execute the project across different platforms.