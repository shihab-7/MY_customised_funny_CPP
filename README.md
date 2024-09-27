# Documentation for Shihab++ Bangla Custom Language Header File

## Overview
This header file defines a custom Bangla C++ language that allows users to write C++ code using Bangla keywords. The goal is to make programming more accessible and enjoyable for Bengali speakers by providing a familiar syntax.

## Features
- **Custom Keywords**: The header file replaces standard C++ keywords with Bangla equivalents.
- **Data Types**: Common C++ data types are represented with Bangla terms.
- **Control Structures**: Conditional statements and loops are expressed in Bangla.
- **Input/Output**: Simplified methods for user input and output in Bangla.

## Installation
To use this header file in your C++ projects:
1. Download the `Shihab++.h` file.
2. Include it in your C++ source file with the following directive:
   ```cpp
   #include "Shihab++.h"
   ```

## Keywords

| Bangla Keyword            | C++ Equivalent       | Description                                |
|---------------------------|----------------------|--------------------------------------------|
| `ashol_khela_shuru`      | `int main()`         | Defines the main function.                 |
| `khela_sesh`             | `return 0;`          | Ends the program.                          |
| `jodi`                   | `if`                 | Conditional statement.                     |
| `nahoy`                  | `else`               | Alternative branch for if statement.      |
| `jotokkhon`              | `while`              | Starts a while loop.                       |
| `thamish_na`             | `do`                 | Starts a do-while loop.                    |
| `kono_ak_karone`         | `for`                | Starts a for loop.                         |
| `shotti`                 | `true`               | Boolean true value.                        |
| `mittha`                 | `false`              | Boolean false value.                       |
| `faka`                   | `void`               | Represents a void function.                |
| `kisu_de`                | `return`             | Returns a value from a function.          |
| `r_a_bondo_kor`          | `break`              | Exits from a loop.                         |
| `chalay_ja`              | `continue`           | Skips to the next iteration of a loop.    |
| `palta`                  | `switch`             | Starts a switch statement.                 |
| `hoyto`                  | `case`               | Defines a case in a switch statement.     |
| `jonmo_theke`            | `default`            | Default case in a switch statement.       |
| `chesta_kor`             | `try`                | Starts a try block for exception handling. |
| `thela_shamla`           | `catch`              | Starts a catch block for handling exceptions. |
| `jukto_kor`              | `include`            | Includes header files.                     |

## Data Types

| Bangla Type               | C++ Equivalent       | Description                                |
|---------------------------|----------------------|--------------------------------------------|
| `gota_sonkha`             | `int`                | Integer data type.                         |
| `soto_doshomic`          | `float`              | Floating-point data type.                 |
| `boro_doshomic`          | `double`             | Double precision floating-point.          |
| `okkhor`                 | `char`               | Character data type.                      |
| `boltesi`                | `string`             | String data type.                         |
| `shotti_mittha`          | `bool`               | Boolean data type.                        |
| `kisu_na`                | `nullptr`            | Represents a null pointer.                |
| `laga_vector`            | `vector`             | Standard vector container.                |
| `laga_list`              | `list`               | Standard list container.                  |
| `laga_map`               | `map`                | Standard map container.                   |
| `laga_set`               | `set`                | Standard set container.                   |

## Control Structures
You can use the following control structures in your code:

- **Conditionals**:
    ```cpp
    jodi (condition) lekha_shuru
        // code if true
    nahoy lekha_shuru
        // code if false
    sesh
    ```

- **Loops**:
    - **While Loop**:
      ```cpp
      jotokkhon (condition) lekha_shuru
          // code to execute
      sesh
      ```
    - **For Loop**:
      ```cpp
      kono_ak_karone (initialization; condition; increment) lekha_shuru
          // code to execute
      sesh
      ```

## Input/Output
Use the following methods for input and output:

- **Output**:
    ```cpp
    dekhi "Hello, World!" notun_line;  // Prints Hello, World!
    ```

- **Input**:
    ```cpp
    assa_ne variable;  // Takes input and stores it in 'variable'
    ```

## Exception Handling
To handle exceptions, use `chesta_kor` and `thela_shamla`:

```cpp
chesta_kor lekha_shuru
    // code that might throw an exception
sesh
thela_shamla e lekha_shuru
    dekhi "Kichu vul hoyeche: " jog e.what() notun_line;  // Print error message
sesh
```

## Examples
Here are some basic examples of using the custom language:

### Example 1: Adding Two Numbers
```cpp
ashol_khela_shuru lekha_shuru
    gota_sonkha a, b;
    dekhi "Prothom shonkha din: " notun_line;
    assa_ne a;
    dekhi "Ditiyo shonkha din: " notun_line;
    assa_ne b;

    dekhi "Jogfol: " jog (a jog b) notun_line;  // Output the sum
khela_sesh
```

### Example 2: Handling Exceptions
```cpp
ashol_khela_shuru lekha_shuru
    chesta_kor lekha_shuru
        // Some code that may throw an exception
    sesh
    thela_shamla e lekha_shuru
        dekhi "Kichu vul hoyeche: " jog e.what() notun_line;
    sesh
khela_sesh
```

## Conclusion
This documentation serves as a guide to using the Bangla C++ custom language defined in the `Shihab++.h` header file. For more advanced usage and features, refer to the specific implementation details or source code comments.
