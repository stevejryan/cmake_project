# cmake_project
Small example of how to lay out a C++ project using CMake to link libraries to a main binary, setup testing

Typical project structure:
```|-- project_name/
|   |-- CMakeLists.txt
|   |-- build/  # All generated build files
|   |-- bin/
|   |   |-- tools_demo
|   |-- lib/
|   |   |-- libtools.a
|   |-- src/
|   |   |-- CMakeLists.txt
|   |   |-- project_name
|   |       |-- CMakeLists.txt
|   |       |-- tools.h
|   |       |-- tools.cpp
|   |       |-- tools_demo.cpp
|   |-- tests/  # Tests for your code
|   |   |-- test_tools.cpp
|   |   |-- CMakeLists.txt
|   |-- readme.md  # How to use your code```
