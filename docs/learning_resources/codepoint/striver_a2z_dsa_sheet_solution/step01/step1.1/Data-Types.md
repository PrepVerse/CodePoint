---
icon: material/numeric-2-circle
---

<!-- ### Integer Types

| Type Name            | Bytes | Range of Values                             |
|----------------------|-------|---------------------------------------------|
| unsigned short       | 2     | 0 to 65,535                                 |
| short int            | 2     | -32,768 to 32,767                           |
| unsigned short int   | 2     | 0 to 65,535                                 |
| signed short int     | 2     | -32,768 to 32,767                           |
| int                  | 4     | -2,147,483,648 to 2,147,483,647             |
| unsigned int         | 4     | 0 to 4,294,967,295                          |
| signed int           | 4     | -2,147,483,648 to 2,147,483,647             |
| long                 | 4     | -2,147,483,648 to 2,147,483,647             |
| long int             | 8     | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 |
| unsigned long int    | 8     | 0 to 18,446,744,073,709,551,615             |
| signed long int      | 8     | 0 to 18,446,744,073,709,551,615             |
| unsigned long        | 4     | 0 to 4,294,967,295                          |
| long long            | 8     | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 |
| long long int        | 8     | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 |

### Floating-Point Types

| Type Name   | Bytes | Range of Values                     |
|-------------|-------|-------------------------------------|
| float       | 4     | 1.2E-38 to 3.4E+38                  |
| double      | 8     | 2.3E-308 to 1.7E+308                |
| long double | 12    | 3.4E-4932 to 1.1E+4932              |

### Character Types

| Type Name     | Bytes | Range of Values         |
|---------------|-------|-------------------------|
| char          | 1     | -128 to 127 or 0 to 255 |
| unsigned char | 1     | 0 to 255                |
| signed char   | 1     | -128 to 127             | -->


!!! example ""
    === "C++"
        !!! tip "Data_Types.cpp"
            ```cpp linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            int main() {
                // Integer types
                int i = 10; // int
                long l = 1005; // long
                long long ll = 10000005; // long long

                // Floating-point types
                float f = 10.5; // float
                float fi = 10; // float (integer value)

                double d = 1005.5; // double
                double di = 1005; // double (integer value)

                // String input and output
                string s1, s2;
                cin >> s1 >> s2;
                cout << "Print normal string: " << endl;
                cout << "s1: " << s1 << ", and s2: " << s2 << endl << endl;

                // Reading a line of text
                string str;
                getline(cin, str);
                cout << "Print getline string: " << endl;
                cout << "str: " << str;

                // Character types
                char ch = 'A'; // char
                string s = "A"; // string containing a single character

                return 0;
            }
            ```
        ??? success "Output"
            ```
            Akash Singh
            Print normal string: 
            s1: Akash, and s2: Singh

            My Name is Akash Singh.
            Print getline string: 
            str: My Name is Akash Singh.
            ```
    === "Python"
        !!! tip "Data_Types.py"
            ```py linenums="1"
            # Integer variables
            i = 10  # An integer variable i with the value 10
            l = 1005  # A long integer variable l with the value 1005
            ll = 10000005  # A long long integer variable ll with the value 10000005

            # Floating-point variables
            f = 10.5  # A float variable f with the value 10.5
            fi = 10  # Another float variable fi with the value 10 (integer value)

            d = 1005.5  # A double variable d with the value 1005.5
            di = 1005  # Another double variable di with the value 1005 (integer value)

            # String input and output
            s1 = input()  # Read a string into s1 from user input
            s2 = input()  # Read another string into s2 from user input
            print("Print normal string: ")
            print("s1:", s1, ", and s2:", s2)
            print()

            # Reading a line of text
            str = input()  # Read a line of text into the variable str from user input
            print("Print getline string: ")
            print("str:", str)

            # Character variables
            ch = 'A'  # A character variable ch with the value 'A'
            s = "A"  # A string variable s containing the character 'A'
            ```
        ??? success "Output"
            ```
            Akash 
            Singh
            Print normal string: 
            s1: Akash, and s2: Singh

            My Name is Akash Singh.
            Print getline string: 
            str: My Name is Akash Singh.
            ```