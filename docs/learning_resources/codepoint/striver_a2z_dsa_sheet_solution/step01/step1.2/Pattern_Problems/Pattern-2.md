---
icon: material/set-square
---

# 2. Triangle Star Pattern

!!! example "Example"
    !!! question "Pattern 2"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
        &*\\
        &*\; *\\
        &*\; *\; *\\
        &*\; *\; *\; *\\
        &*\; *\; *\; *\; *
        \end{align}
        $$
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                for(int i=0; i<n; i++) {
                    for(int j=0; j<=i; j++) {
                        cout << "* ";
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
            * 
            * * 
            * * * 
            * * * * 
            * * * * *
            ```