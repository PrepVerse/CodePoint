---
icon: material/numeric-6-box
---

!!! example ""
    ## Method-1
    === "C++"
        ???+ tip "print_Divisor.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void print_Divisor(int n){
                cout << "All Divisors are: ";
                for(int i=1; i<=n; i++) {
                    if(n%i == 0) {
                        cout << i << " ";
                    }
                }
                cout << endl;
            }

            int main() {
                int n;
                cin >> n;
                print_Divisor(n);
                return 0;
            }
            ```
            /// html | div.result
            ++'Input'++: 36 <br>
            ++'Output'++: All Divisors are: 1 2 3 4 6 9 12 18 36
            ///
    ## Method-2
    === "C++"
        ???+ tip "print_Divisor.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void print_Divisor(int n){
                cout << "All Divisors are: ";
                for(int i=1; i<=sqrt(n); i++) {
                    if(n%i == 0) {
                        cout << i << " ";
                        if(i != n/i) {
                            cout << n/i << " "; 
                        }
                    }
                }
                cout << endl;
            }

            int main() {
                int n;
                cin >> n;
                print_Divisor(n);
                return 0;
            }
            ```
            /// html | div.result
            ++'Input'++: 36 <br>
            ++'Output'++: All Divisors are: 1 2 3 4 6 9 12 18 36
            ///