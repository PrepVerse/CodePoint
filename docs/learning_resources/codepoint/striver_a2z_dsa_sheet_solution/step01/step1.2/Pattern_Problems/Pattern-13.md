---
icon: material/set-square
---

# 13. Triangle Digit Pattern

!!! example "Example"
    !!! question "Pattern 13"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
        &1\\
        &2\; 3\\
        &4\; 5\; 6\\
        &7\; 8\; 9\; 10\\
        &11\; 12\; 13\; 14\; 15
        \end{align}
        $$
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                int num=1;
                for(int i=1; i<=n; i++) {
                    for(int j=0; j<i; j++) {
                        cout << num++ << " ";
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
            2 3 
            4 5 6 
            7 8 9 10 
            11 12 13 14 15
            ```