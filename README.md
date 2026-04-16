# C++ Windows Program

## Overview

This is a simple C++ program built for Windows using standard libraries and the Windows API.

The goal of this project is to provide a **portable executable (.exe)** that users can run **without installing additional libraries or dependencies**.

---

## Features

* Uses Windows API (`windows.h`)
* File handling (`fstream`)
* Console input/output (`iostream`)
* Basic character processing (`cctype`)

---

## Requirements (for developers)

To build this project, you need:

* A C++ compiler (e.g., MinGW or MSVC)
* Windows OS

---

## Build Instructions

### Using g++ (MinGW)

Compile the program with static linking:

```bash
g++ run.cpp -o program.exe -static -static-libgcc -static-libstdc++
```

### Using Visual Studio

1. Open the project in Visual Studio
2. Go to:

   * Project Properties → C/C++ → Code Generation
3. Set:

   * Runtime Library → **Multi-threaded (/MT)**
4. Build the project

---

## Running the Program

After building, you will get:

```
program.exe
```

Users can run it directly:

```bash
./program.exe
```

No additional installations are required.

---

## Distribution

To distribute your program:

* Share only the `.exe` file
* No need to include DLLs if statically linked

---

## Notes

* Static linking increases file size
* Works only on Windows
* Ensure testing on a clean system before distribution

---

## License

This project is open for personal and educational use.

---

## Note

The executable file runs in the background and store keys in a .txt file if you want to close the program. go to task manager > run.exe > end process

---

## Author

Created by noniCoder
