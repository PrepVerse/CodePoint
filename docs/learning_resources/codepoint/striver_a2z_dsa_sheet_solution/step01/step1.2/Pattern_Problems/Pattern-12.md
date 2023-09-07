# 11. Left-Right Triangle Digit Pattern

!!! example "Example"
    !!! question "Pattern 12"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
            &1 \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad 1 \\
            &1 \quad 2 \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad 2 \quad 1 \\
            &1 \quad 2 \quad 3 \quad \quad \quad \quad \quad \quad \quad 3 \quad 2 \quad 1 \\
            &1 \quad 2 \quad 3 \quad 4 \quad \quad \quad \quad 4 \quad 3 \quad 2 \quad 1 \\
            &1 \quad 2 \quad 3 \quad 4 \quad 5 \quad 5 \quad 4 \quad 3 \quad 2 \quad 1 \\
        \end{align}
        $$
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                for(int i=1; i<=n; i++) {
                    for(int j=1; j<=i; j++) {
                        cout << j << " ";
                    }
                    for(int k=0; k<4*(n-i); k++) {
                        cout << " ";
                    }
                    for(int j=i; j>0; j--) {
                        cout << j << " ";
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
            1                 1
            1 2             2 1
            1 2 3         3 2 1
            1 2 3 4     4 3 2 1
            1 2 3 4 5 5 4 3 2 1
            ```