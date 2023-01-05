!!! example "Example"
    === "C++"
        ???+ tip "printSquare.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printSquare(int n) {
                for(int i=n; i>0; i--) {
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
            **********
            ****  ****
            ***    ***
            **      **
            *        *
            *        *
            **      **
            ***    ***
            ****  ****
            **********
            ```