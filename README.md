# Workshop 1. How to build a simple "Hello world" program in C++

S. Shershakov, G. Zhulikov

January 09, 2023

###  Goals

Understanding the process of building C++ programs with CMake meta-building system.


## Description

Tools which need to be installed and configured to develop C++ applications:

- a **toolchain** - a C++ compiler and related built-in tools.
- a **building system** - management tool for complex projects.
- an **IDE** - integrated development environment. Software that combines text editing and integration with other tools.

In this course, we will use the following:

- **Visual Studio Code** as the text editor and IDE. https://code.visualstudio.com
  - By itself it's a text editor, but with `C/C++` and `CMake Tools` extensions it starts being similar to an IDE.
- **gcc/clang** as the toolchain.
  - on Windows it's MinGW, a port of gcc. Instructions - https://www.msys2.org/ and https://code.visualstudio.com/docs/cpp/config-mingw
  - on Mac `clang` might be pre-installed. Try `clang --version` in Terminal. If it't not installed, run the command `xcode-select --install`

- **CMake** as the building system. Download - https://cmake.org/download. Look for "Binary distributions" for your system.
  - There are some instructions here - https://code.visualstudio.com/docs/cpp/cmake-linux. It says "on Linux" but almost all steps are the same for all platforms.

## Files

## Exercises

1. Study the structure of the project
2. Study the contents of `/workshop1/src/CMakeLists.txt` file. This is an entry point for building your applications. Discuss the content with your instructor.
3. Open the **directory** `workshop1` in VS Code. It should open as a project. If you use another IDE, you should open `/workshop1/src/CMakeLists.txt` as a project. Consult with your instructor that you opened it correctly. VS Code should suggest to "configure the project".
4. Configure the project. Keep default settings. For VS Code it means clicking "Yes" in the prompt. If there was no prompt, press `Ctrl+Shift+P` (or `Cmd+Shift+P`) and type `CMake: Configure` - the option should appear in the list.
5. **Build** your applications. Use the button "Build" at the bottom of the screen in VS Code.
6. Find the application you built in your project's directory in the file system. It should be a file called `ex1` or `ex1.exe`. Run this file and observe the output. The output should be "Hello world!".
7. Modify the code according to instructions from your workshop instructor. Rebuild the application and check that the output changes correctly.
   - For example: change the message, input a number and print it back, don't print anything, etc.
8. Follow instructions from directory `workshop1/ex2` and make a second application.
9. Practice debugging according to instructions from your workshop instructor.
