---
icon: material/set-square
---

# 14. Triangle Character Pattern

!!! example "Example"
    !!! question "Pattern 14"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
        &A\\
        &AB\\
        &ABC\\
        &ABCD\\
        &ABCDE\\
        \end{align}
        $$
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                for(int i=1; i<=n; i++) {
                    char ch = 'A';
                    for(int j=0; j<i; j++) {
                        cout << ch++;
                    }
                    cout << endl;
                }
            }

            int main(void) {
                int n;
                cin >> n;
                printTriangle(n);
                return 0;
            }
            ```
            /// html | div.result
            ++'Input'++: 5 <br>
            ++'Output'++:
            ```
            A
            AB
            ABC
            ABCD
            ABCDE
            ```