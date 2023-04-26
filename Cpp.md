# C++

Personal C++ style guide, program structure

SUBJECT TO CHANGE

## (Personal) style guide

Naming
- Non-const Variables and Functions
  - Use mixedCase
  - Ex. `engine`, `carBrand`, `horsePower`
- Const Variables
  - Use ALLCAPS
  - Ex. `MAXRPM`, `GRAVITY`, `FRICTION`
- Classes and Structs
  - Use CamelCase
  - Ex. `Plane`, `JetEngine`, `PlaneWings`

Files
- use `.cpp` for source code and `.hpp` for header files
- header guard template
  -  ```cpp
     #ifndef [nameNoExtension]_HPP
     #define [nameNoExtension]_HPP
     
     // code
     
     #endif
     ```
  - Ex for `[nameNoExtensoin]_HPP`: `RENDER_HPP` for file `render.hpp` 
- `#Include` order
  - ```cpp
    // project source files
    // libraries used
    // standard library
    ```
  - use quotes on everything except for standard library includes
  - libraries used would be `"Raylib.h"` if I was using the raylib library
  - Standard library would be things like `<iostream>` and `<vector>`
