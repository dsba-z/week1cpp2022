# Exercise 2. Multi-file project.

Create three files in this directory: `main.cpp`, `foo.cpp`, `foo.h`.

`main.cpp` is a startup module, it should include `foo.h` and call function `foo()`.

`foo.h` is a header, it should contain a *protorype/declaration* of a function `int foo();`

`foo.cpp` is a module with an *implementation* the function `foo()`.

Example of implementation:

```cpp
int foo()
{
    return 123;
}
```

Uncomment the line `# add_executable(ex2 ex2/main.cpp ex2/foo.cpp ex2/foo.h)` in **CMakeLists.txt**.

Build your application. Choose `ex2` as your target (the button next to "Build"). It may not appear there instantly. If your have trouble, try configuring the project again.
