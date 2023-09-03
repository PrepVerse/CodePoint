!!! example "Example"
    !!! question "Pattern 7"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
                &*\\
               &***\\  
              &*****\\
             &*******\\
            &*********
        \end{align}
        $$
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                for(int i=1; i<=n; i++) {
                    for(int k=0; k<(n-i); k++) {
                        cout << " ";
                    }
                    for(int col=0; col<2*row-1; col++) {
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
                *
               ***  
              *****
             *******
            *********
            ```