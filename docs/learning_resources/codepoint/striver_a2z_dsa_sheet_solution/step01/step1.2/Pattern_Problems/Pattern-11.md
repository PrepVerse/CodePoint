---
icon: material/set-square
---

# 11. Triangle Digit Pattern

!!! example "Example"
    !!! question "Pattern 11"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
        &1\\
        &0\; 1\\
        &1\; 0\; 1\\
        &0\; 1\; 0\; 1\\
        &1\; 0\; 1\; 0\; 1
        \end{align}
        $$
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                for(int i=1; i<=n; i++) {
                    for(int j=0; j<i; j++) {
                        if((i+j)%2 == 0)
                            cout << "0 ";
                        else
                            cout << "1 ";
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
            1 
            0 1 
            1 0 1
            0 1 0 1 
            1 0 1 0 1
            ```