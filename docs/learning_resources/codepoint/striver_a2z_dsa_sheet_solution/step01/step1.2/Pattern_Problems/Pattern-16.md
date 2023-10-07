---
icon: material/set-square
---

# 16. Triangle Character Pattern

!!! example "Example"
    !!! question "Pattern 16"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
        &A\\
        &BB\\
        &CCC\\
        &DDDD\\
        &EEEEE\\
        \end{align}
        $$
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                char ch = 'A';
                for(int i=1; i<=n; i++) {
                    for(int j=0; j<i; j++) {
                        cout << ch;
                    }
                    ch++;
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
            BB
            CCC
            DDDD
            EEEEE
            ```