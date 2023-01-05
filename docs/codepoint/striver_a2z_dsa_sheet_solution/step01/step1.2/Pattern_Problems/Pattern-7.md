!!! example "Example"
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
                    for(int j=0; j<2*i-1; j++) {
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