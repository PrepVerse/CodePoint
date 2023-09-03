!!! example "Example"
    !!! question "Pattern 20"
        <h1 align="center">$N = 5$</h1>

        $$\Large
        \begin{align}
            &\ast\ \ \ \ \ \ \ \  \ \ \ \ \ \ \  \ \ \ \ \ \ \ \ \ \ast \\
            &\ast\ast\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ast\ast \\
            &\ast\ast\ast\ \ \ \ \ \ \ \ \ \ \ \ \ast\ast\ast \\
            &\ast\ast\ast\ast\ \ \ \ \ \ \ast\ast\ast\ast \\
            &\ast\ast\ast\ast\ast\ast\ast\ast\ast\ast \\
            &\ast\ast\ast\ast\ \ \ \ \ \ \ast\ast\ast\ast \\
            &\ast\ast\ast\ \ \ \ \ \ \ \ \ \ \ \ \ast\ast\ast \\
            &\ast\ast\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ast\ast \\
            &\ast\ \ \ \ \ \ \ \  \ \ \ \ \ \ \  \ \ \ \ \ \ \ \ \ \ast \\
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
                        cout << "*";
                    }
                    for(int j=0; j<2*(n-i); j++) {
                        cout << " ";
                    }
                    for(int j=0; j<i; j++) {
                        cout << "*";
                    }
                    cout << endl;
                }
                for(int i=n-1; i>0; i--) {
                    for(int j=0; j<i; j++) {
                        cout << "*";
                    }
                    for(int j=0; j<2*(n-i); j++) {
                        cout << " ";
                    }
                    for(int j=0; j<i; j++) {
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
            *        *
            **      **
            ***    ***
            ****  ****
            **********
            ****  ****
            ***    ***
            **      **
            *        *
            ```