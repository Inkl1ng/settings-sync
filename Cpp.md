# C++

Personal C++ style guide, program structure  
Currently WIP, still figuring out how I like to do certain things

**RULE 0: KEEP IT CONSISTENT**  
if you break the guidelines then at least consistently break them

SUBJECT TO CHANGE

## (Personal) style guide
### Tabs/Spaces
- Use spaces over tabs
- set tabs = 4 spaces

### Naming
- Non-const Variables and Functions
  - Use mixedCase
  - Ex. `engine`, `carBrand`, `horsePower`
- Const Variables
  - Use ALLCAPS
  - Ex. `MAXRPM`, `GRAVITY`, `FRICTION`
- Classes and Structs
  - Use CamelCase
  - Ex. `Plane`, `JetEngine`, `PlaneWings`

### Files
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
    // corresponding header file for .cpp files
    // project source files
    // libraries used
    // standard library
    ```
  - use quotes on everything except for standard library includes
  - libraries used would be `"Raylib.h"` if I was using the raylib library
  - Standard library would be things like `<iostream>` and `<vector>`
  - don't make a fuss about order

### Formatting
Braces
- put openning curly brace `{` on same line for `if`, `for`, etc.
- put closing curly brace `}` on new line
- initialize variables with curly braces
  - Ex. `int horsepower { 800 };`
  - its safer
  - make sure to put a space after the variable name and spaces seperating the value of the variable with the curly braces
- 
