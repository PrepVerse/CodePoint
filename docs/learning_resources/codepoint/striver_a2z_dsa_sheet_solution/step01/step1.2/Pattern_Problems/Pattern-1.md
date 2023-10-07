---
icon: material/square
---

# 1. Square Star Pattern

!!! example "Example"
    !!! question "Pattern 1"
        <h1 align="center">$N = 5$</h1>

        $$\Large
        \begin{align}
        * * * * *\\
        * * * * *\\
        * * * * *\\
        * * * * *\\
        * * * * *
        \end{align}
        $$
    === "C++"
        ???+ tip "printSquare.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printSquare(int n) {
                for(int i=0; i<n; i++) {
                    for(int j=0; j<n; j++) {
                        cout << "* ";
                    }
                    cout << endl;
                }
            }

            int main(void) {
                int n;
                cin >> n;
                printSquare(n);
                return 0;
            }
            ```
            /// html | div.result
            ++'Input'++: 5 <br>
            ++'Output'++:
            ```
            * * * * *
            * * * * *
            * * * * *
            * * * * *
            * * * * *
            ```