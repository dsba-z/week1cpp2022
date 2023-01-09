# Notes for the package

This folder plays role of a so-called "package".

The `src` subdirectory contains all necessary sources including the `CMakeLists.txt` file that is the an entry point to an application build system.

When you configure the output of your building system, consider to put it next to the `/src` directory. E.g. it can be in the `/build` folder. Never put the outcome in the directory with sources, namely `/src`, because it this contradicts the "directory separating" approach of CMake and will make a mess out of your project.

By default VS Code should put outputs to `/build`, so you don't have to configure it.
