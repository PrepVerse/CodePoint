---
icon: material/numeric-5-circle
---

!!! example
    !!! abstract "Arrays"
        1. **Definition:** An array is a data structure that stores a fixed-size, ordered collection of elements of the same data type. Each element in an array is identified by its index or position.

        2. **Features:**
            - **Fixed Size:** Arrays have a predetermined size when they are declared, and this size cannot be changed during runtime.
            - **Homogeneous:** All elements in an array must be of the same data type (e.g., integers, floats, characters).
            - **Indexed:** Elements in an array are accessed using an index, starting from 0 for the first element.
            - **Contiguous Memory:** Array elements are stored in contiguous memory locations.

        3. **Examples:**
            - Integer Array: `int numbers[5];`
            - Character Array (String): `char greeting[10];`

        4. **Common Operations:**
            - Accessing Elements: `array[index]`
            - Modifying Elements: `array[index] = value`
            - Iterating through Elements: Using loops (e.g., `for` loop)
            - Finding Length: `sizeof(array) / sizeof(array[0])`

    !!! abstract "Strings"
        1. **Definition:** A string is a sequence of characters, represented as an array of characters. In many programming languages, strings are treated as a special type of array with built-in functions for text manipulation.

        2. **Features:**
            - **Variable Length:** Strings can vary in length, and their size can change during runtime.
            - **Characters:** Strings are composed of characters, typically represented using the `char` data type.
            - **Null-Terminated:** In C-style strings, a null character (`'\0'`) marks the end of the string.

        3. **Examples:**
            - C-style String: `char greeting[] = "Hello";`
            - String in Python: `"Hello, World"`

        4. **Common Operations:**
            - Concatenation: Combining two or more strings (e.g., `"Hello, " + "World"`)
            - Length: Finding the number of characters in a string (e.g., `strlen` in C/C++)
            - Comparison: Checking if two strings are equal (e.g., `"abc" == "def"`)
            - Substring: Extracting a portion of a string (e.g., `"Hello".substring(1, 3)` in Java)

    === "C++ : Array _ METHOD-1"
        !!! tip "Array.cpp"
            ```c++ linenums="1" hl_lines="5-9"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                int a, b, c, d, e
                cin >> a >> b >> c >> d >> e;

                int sum = a + b + c + d + e;
                cout << sum;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            1 2 3 4 5
            15
            ```
    === "C++ : Array _ METHOD-2"
        !!! tip "Array.cpp"
            ```c++ linenums="1" hl_lines="5-9"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                int arr[5];
                cin >> arr[0] >> arr[1] >> arr[2] >> arr[3] >> arr[4];

                int sum = arr[0] + arr[1] + arr[2] + arr[3] + arr[4];
                cout << sum;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            1 2 3 4 5
            15
            ```
    === "C++ : 2D Array _ METHOD-1"
        !!! tip "Matrix.cpp"
            ```c++ linenums="1" hl_lines="5-9"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                int arr[2][2];
                cin >> arr[0][0] >> arr[0][1] >> arr[1][0] >> arr[1][1];

                int sum = arr[0][0] + arr[0][1] + arr[1][0] + arr[1][1];
                cout << sum;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            1 2 3 4
            10
            ```
    === "C++ : String _ METHOD-1"
        !!! tip "String.cpp"
            ```c++ linenums="1" hl_lines="5-7"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                string str = "Akash Singh";
                int len = str.size();
                cout << str[len-1];
                return 0;
            }
            ```
        ??? success "Output"
            ```
            h
            ```

