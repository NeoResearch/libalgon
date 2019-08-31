# libalgon

## Verifiable Algorithms for Neo Blockchain

This project is part of the [neopt](https://github.com/neoresearch/neopt) macro project, a C++ implementation of Neo Blockchain components, focused on portability.

## Why chosing C/C++ language for that?
Existing frameworks use high-level languages that may not be suitable for very lightweight architectures,
such as microcontrollers with very limited computing capabilities.

C/C++ is interoperable with nearly all existing languages, so the idea is to provide modules that can be
reused on other projects (on other languages too).

**Note:** this project is still being __ported out__ of neopt, since other community projects have interest in using this special component in a very separate manner. In a few days, much more things should be here ;)

## Build Instructions
This project depends on `libcrypton`, to provide cryptographic functions.

### tests

It will also configure test library (as long as you cloned this project with `--submodules` too).
To test, just run `make test`.


## C++ Standard
Currently, C++11 is adopted, in order to keep the best compatibility between conversors and compilers. However, it is recommended to migrate to C++17 as soon as possible, if this does not break compatibility with any existing modules and tools.

Let's please follow the [CppCoreGuidelines](https://github.com/isocpp/CppCoreGuidelines).

#### vscode IDE
If using vscode IDE, it is recommended to install the following extensions:
* C/C++ (currently 0.23.0-insiders2)
* C++ Intellisense (currently 0.2.2)
* GoogleTest Adapter (currently 1.8.3)

#### C++ Format Style
The currently adopted style for C++ is `Mozilla`, with indentation level set to 3.
Recommended configuration for vscode:
```json
{
    "[cpp]": {
        "editor.tabSize" : 3,
        "editor.detectIndentation": false
    },
    "C_Cpp.clang_format_fallbackStyle": "{ BasedOnStyle : Mozilla , ColumnLimit : 0, IndentWidth: 3, AccessModifierOffset: -3}"
}
```

### License

Code follows `MIT License`.

