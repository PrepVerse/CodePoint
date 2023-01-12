!!! example "Example"
    === "C++"
        ???+ tip "printSquare.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printSquare(int n) {
                for(int i=1; i<=n; i++) {
                    for(int j=1; j<=n; j++) {
                        if(i==1 or i==n or j==1 or j==n) {
                            cout << "*";
                        } 
                        else {
                            cout << " ";
                        }
                    }
                    cout << endl;
                }
            }

            int main(void) {
                int n;
                cin >> n;
                printSquare(n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5
            *****
            *   *
            *   *
            *   *
            *****
            ```