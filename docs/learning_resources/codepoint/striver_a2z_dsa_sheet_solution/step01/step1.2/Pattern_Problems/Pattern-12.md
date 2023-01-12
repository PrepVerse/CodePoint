!!! example "Example"
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