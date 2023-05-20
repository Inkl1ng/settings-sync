# C++

Personal C++ style guide, program structure  
Currently WIP, still figuring out how I like to do certain things

**RULE 0: KEEP IT CONSISTENT**  
if you break the guidelines then at least consistently break them

SUBJECT TO CHANGE

## (Personal) style guide
### General
- Use spaces over tabs
- Set tabs = 4 spaces
- Put openning brace `{` on same line and closing brace `}` on new line
- Try to keep lines under 80 characters and 72 for docstrings
  - Doesn't have to be always followed, can go a little bit over
  - Max 100 characters
- Use `.cpp` file extension for source files and `.hpp` for header files
- `#include` order: source headers, library headers, standard library
  - No order within the categories

### Naming
Element | Convention | Example
--- | :---: | ----
Variables | snake_case | `bool is_frozen = false;`
Const Variable | snake_case | `const int screen_height = 1080;`
Functions | lowerCase | `void addScore()`
Function Parameters | snake_case | `double new_color`
Classes | TitleCase | `class PickupTruck`
Attributes | snake_case | `int engine_horsepower;`
Methods | TitleCase | `bool IsEngineBroken()`
Structs | TitleCase | `struct 3dPoint`
Struct Members | snake_case | `int x_coordinate;`
Enum | TitleCase | `enum Colors`
Enum Members | ALL_CAPS | `BLUE,`
Pointers | Type* variable_name | `Player* player_1;`
References | Type& variable_name | `Player& player_1;`

### Header Files
- Only put declarations
  - Exceptions: templates
- header guard template
  -  ```cpp
     #ifndef [nameNoExtension]_HPP
     #define [nameNoExtension]_HPP
     
     // code
     
     #endif
     ```
  - Ex for `[nameNoExtensoin]_HPP`: `RENDER_HPP` for file `render.hpp` 
