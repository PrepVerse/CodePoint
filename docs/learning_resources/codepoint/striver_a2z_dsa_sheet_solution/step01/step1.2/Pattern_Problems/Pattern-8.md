!!! example "Example"
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