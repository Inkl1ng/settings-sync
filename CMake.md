# CMake

**DISCLAIMER: MIGHT NOT BE THE BEST WAY TO DO THINGS, THESE ARE JUST WHAT I DO**

For CMake related things, mostly CMakeLists.txt related things.
Regular C++ program structure (for reference)  
- /ProjectDir/  
    - /bin/  
    - /src/  
    - [git-related files]<br>

So far my projects haven't required me to stray from this norm but this will probably change later in the future  


## Starter template for project

```CMake
cmake_minimum_required(VERSION <CMAKE_VERSION_NUMBER>)

project(<PROJECT_NAME> VERSION <PROJECT_VERSION_NUMBER>)

add_executable(<PROJECT_NAME> 
    <list files that need to be compilied for the executable here>)
```
replace the things in `<>`'s with what they should be

### Notes
  - usually put 3.0 or 3.1 for `<CMAKE_VERSION_NUMBER>`
  - list files for compilation on a seperate line from the project name
    - list `"main.cpp" first
    - haven't decided whether to make a new line for each source file
  - file names for compilation need quotation marks and extension name
    - ex. `"render.cpp"`

## Closer to essentials
```CMake
set(EXECUTABLE_OUTPUT_PATH ../bin)
```
  - Sets executable to be outputted into the `[project directory]/bin/`
