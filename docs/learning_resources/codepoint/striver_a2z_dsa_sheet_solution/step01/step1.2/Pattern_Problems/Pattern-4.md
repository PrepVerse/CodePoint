# 4. Triangle Digit Pattern

!!! example "Example"
    !!! question "Pattern 4"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
        &1\\
        &2\; 2\\
        &3\; 3\; 3\\
        &4\; 4\; 4\; 4\\
        &5\; 5\; 5\; 5\; 5
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
                        cout << i+1 << " ";
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
            1
            2 2 
            3 3 3 
            4 4 4 4 
            5 5 5 5 5
            ```