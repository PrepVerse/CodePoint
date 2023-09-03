!!! example "Example"
    !!! question "Pattern 15"
        <h1 align="center">$N = 5$</h1>
        
        $$\Large
        \begin{align}
        &ABCDE\\
        &ABCD\\
        &ABC\\
        &AB\\
        &A\\
        \end{align}
        $$
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                for(int i=n; i>0; i--) {
                    char ch = 'A';
                    for(int j=0; j<i; j++) {
                        cout << ch++;
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
            ABCDE
            ABCD
            ABC
            AB
            A
            ```