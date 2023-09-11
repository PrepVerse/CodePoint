---
icon: material/numeric-8-circle
---

!!! example ""
    !!! abstract "Use of functions"
        1. Functions are set of code wich performs somethig for you
        2. Functions are used to modularised code
        3. Functions are used to increase readability
        4. Functions are used to use same code multiple times
    !!! note "Type of functions"
        1. void --> which does not return annything
        2. parameterised
        3. non parameterised
        4. return
        5. Pass by Value
        6. Pass by Refrence
    
    ## Void - Non_Parameterised
    === "C++"
        !!! tip "Void_Function.cpp"
            ```c++ linenums="1" hl_lines="4-6 9"
            #include<bits/stdc++.h>
            using namespace std;

            void printName() {
                cout << "Akash Singh";
            }

            int main() {
                printName();
                return 0;
            }
            ```
        ??? success "Output"
            ```
            Akash Singh
            ```
    ## Void - Parameterised
    === "C++"
        !!! tip "Parameterised_Function.cpp"
            ```c++ linenums="1" hl_lines="4-6 9-11"
            #include<bits/stdc++.h>
            using namespace std;

            void printName(string name) {
                cout << "Hello " << name;
            }

            int main() {
                string name;
                cin >> name;
                printName(name);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            Akash
            Hello Akash
            ```
    ## Return - Parameterised
    === "C++"
        !!! tip "Return_Function.cpp"
            ```c++ linenums="1" hl_lines="4-7 10-12"
            #include<bits/stdc++.h>
            using namespace std;

            int Sum(int num1, int num2) {
                int sum = num1 + num2;
                return sum;
            }

            int main() {
                int num1, num2;
                cin >> num1 >> num2;
                cout << Sum(num1, num2);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5 6
            11
            ```
    ## Pass by Value
    === "C++"
        !!! tip "Pass_by_Value.cpp"
            ```c++ linenums="1" hl_lines="4-10 15-16"
            #include<bits/stdc++.h>
            using namespace std;

            void AddFive(int num) {
                cout << "num" << endl;
                num += 5;
                cout << "num" << endl;
                num += 5;
                cout << "num" << endl;
            }

            int main() {
                int num;
                cin >> num;
                AddFive(num);
                cout << num;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            10
            15
            20
            10
            ```
    ## Pass by Refrence
    === "C++"
        !!! tip "Pass_by_Refrence.cpp"
            ```c++ linenums="1" hl_lines="4-10 15-16"
            #include<bits/stdc++.h>
            using namespace std;

            void AddFive(int &num) {
                cout << "num" << endl;
                num += 5;
                cout << "num" << endl;
                num += 5;
                cout << "num" << endl;
            }

            int main() {
                int num;
                cin >> num;
                AddFive(num);
                cout << num;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            10
            15
            20
            20
            ```