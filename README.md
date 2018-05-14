# CppCheatSheet
The repository is a compilation of C++ features examples aimed at those, who are new to C++ or new to modern C++ standards. Each example is located in it's own folder, is commented to provide insight into the feature and is configured with *cmake* (but still it can be compiled using your favourite compiler manually).

The repository will be updated with new examples.

This readme consists of three parts:
- Requirements
- Example descriptions
- License

## Requirements

- cmake
- a C++ compiler

### In Depth description:

The projects are written with running on linux in mind, and are configured with a [*cmake*](https://cmake.org/) script. You can run it on whatever platform you'll make this run, but following description is created for Ubuntu. For examples using modern features you'll need a compiler in a version new enough to support new standards. Software version can be usually checked by providing *--version* flag. For example, to check *gcc* version:

```
$ gcc --version
```
### Compilers:
*gcc* and *clang* versions needed for:
- full support of C++17: 
    - GCC 7 
    - Clang 5
- full support of C++14: 
    - GCC 6.1
    - Clang 3.4
- full support of C++11: 
    - GCC 4.8.1
    - Clang 3.3

More info about these compilers statuses can be found [here (gcc)](https://gcc.gnu.org/projects/cxx-status.html) and [here (clang)](https://clang.llvm.org/cxx_status.html).  
Mentioned standards can be used in earlier versions of compilers with partially implemented functionalisties, by providing:
- *--std=c++1x* for "not finished" C++11
- *--std=c++1y* for "not finished" C++14
- *--std=c++1z* for "not finished" C++17
- *--std=c++2a* for "not finished" C++20

On Ubuntu, gcc should be installed by default, but can be installed alongside other building tools by calling:

```
$ sudo apt-get install build-essential
```

To install Clang:

```
$ sudo apt-get install clang
```

Keep in mind, that updating repositories list before installing any package could be a good idea. To do this run:

```
$ sudo apt-get update
```

### cmake:
 
To install *cmake*:

```
$ sudo apt-get install cmake
```
To compile exmaple, go to the example's root folder and run following commands:

```
$ cmake CMakeLists.txt
$ make
```
Files and tools needed to compile should be automatically detected and compiled


 Cmake will take your default C++ compiler. It can be changed by adding following line to the *CMakeLists.txt* in the examlple root folder:

```
SET(CMAKE_CXX_COMPILER /path/to/cpp/compiler)
```

## License

Code published in this repository is under **Beerware** license. You are free to do whatever you want with published code snippets and software under one condition: if you would meet the author of example you found useful, you can buy her/him a beer in return. 
