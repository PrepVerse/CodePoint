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


!!! example "C++ Example"
    === "C++"
        !!! tip "Data_Types.cpp"
            ```cpp linenums="1" hl_lines="5-6 8-9 11-12 14-16 18-20 22-24 28-30 34-36"
            #include <bits/stdc++.h>
            using namespace std;

            int main() {
                // int
                int i = 10;

                // long
                long l = 1005;

                // long long
                long long ll = 10000005;

                // float
                float f = 10.5;
                float fi = 10;

                // double
                double d = 1005.5;
                double di = 1005;

                // string
                string s1, s2;
                cin >> s1 >> s2;
                cout << "Print normal string: " << endl;
                cout << "s1: " << s1 << ", and s2: " << s2 << endl << endl;

                // getline
                string str;
                getline(cin, str);
                cout << "Print getline string: " << endl;
                cout << "str: " << str;

                // char
                char ch = 'A';
                string s = "A";

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


!!! example "Python Example"
    === "Python"
        !!! tip "Data_Types.py"
            ```py linenums="1" hl_lines="1-2 4-5 7-8 10-12 14-16 18-22 24-27 29-31"
            # int
            i = 10;

            # long
            l = 1005;

            # long long
            ll = 10000005;

            # float
            f = 10.5;
            fi = 10;

            # double
            d = 1005.5;
            di = 1005;

            # string
            s1, s2 = input(), input();
            print("Print normal string: ");
            print("s1:", s1, ", and s2:", s2);
            print()

            # getline
            str = input();
            print("Print getline string: ")
            print("str:", str)

            # char
            ch = 'A';
            s = "A";
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