!!! example "Example"
    === "C++"
        ???+ tip "printDiamond.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printDiamond(int n) {
                for(int i=1; i<=n; i++) {
                    for(int j=0; j<n-i; j++) {
                        cout << " ";
                    }
                    for(int k=0; k<i; k++) {
                        cout << "* ";
                    }
                    cout << endl;
                }
                for(int i=n; i>0; i--) {
                    for(int j=n-i; j>0; j--) {
                        cout << " ";
                    }
                    for(int k=0; k<i; k++) {
                        cout << "* ";
                    }
                    cout << endl;
                }
            }

            int main(void) {
                int n;
                cin >> n;
                printDiamond(n);
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
            *********
             *******
              *****
               ***
                *
            ```