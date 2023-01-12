!!! example "Example"
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                for(int i=1; i<=n; i++) {
                    char ch = 'A';
                    for(int j=0; j<n; j++) {
                        ch++;
                    }
                    for(int j=0; j<i; j++) {
                        cout << --ch << " ";
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
            E
            E D
            E D C
            E D C B
            E D C B A
            ```