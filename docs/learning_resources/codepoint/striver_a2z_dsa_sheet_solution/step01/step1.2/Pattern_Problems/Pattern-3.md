# 3. Triangle Digit Pattern

!!! example "Example"
    !!! question "Pattern 3"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
        &1\\
        &1\; 2\\
        &1\; 2\; 3\\
        &1\; 2\; 3\; 4\\
        &1\; 2\; 3\; 4\; 5
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
                        cout << j+1 << " ";
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
            1 2 
            1 2 3 
            1 2 3 4 
            1 2 3 4 5
            ```