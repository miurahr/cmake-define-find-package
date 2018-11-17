# Define custom script as same functionality as Find module.

This is meta function module to define  `find_package2()` and
`define_find_package(<name> <header file name> <library name>)`

## How to use?

1. Place cmake scripts under `Modules` folder in your project and add search path
in your `CMakeLists.txt` by setting `CMAKE_MODULE_PATH` variable.
2. Include script using `include(DefineFindPackage2)` in your `CMakeLists.txt`
3. Call function 
   `define_find_package(<name> <header file name> <library name>)`
4. Call `find_package2()` funtion as similar syntax as `find_pacakge()`
5. You can get `<Upper-case name>::<name>` imported target as well as
   `<name>_FOUND`, `<name>_LIBRARIES` and `<name>_INCLUDE_DIRS`.

## License

This is distributed under OSI-Approved 3-Clause BSD license.
