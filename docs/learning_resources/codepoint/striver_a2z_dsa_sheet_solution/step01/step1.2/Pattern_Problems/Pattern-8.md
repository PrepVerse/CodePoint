---
icon: material/triangle-down
---

# 8. Reverse Triangle Star Pattern

!!! example "Example"
    !!! question "Pattern 8"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
            &\phantom{}*********\\
            &\phantom{*}*******\\
            &\phantom{**}*****\\
            &\phantom{***}***\\
            &\phantom{****}*\\
        \end{align}
        $$
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                for(int i=n; i>0; i--) {
                    for(int j=n-i; j>0; j--) {
                        cout << " ";
                    }
                    for(int k=0; k<2*i-1; k++) {
                        cout << "*";
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
        ??? success "Output"
            ```
            5
            *********
             *******
              *****
               ***
                *
            ```