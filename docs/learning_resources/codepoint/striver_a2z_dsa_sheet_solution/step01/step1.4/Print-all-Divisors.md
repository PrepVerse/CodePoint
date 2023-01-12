!!! example "Example"
    === "C++ : METHOD-1"
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
        ??? success "Output"
            ```
            36
            All Divisors are: 1 2 3 4 6 9 12 18 36
            ```
    === "C++ : METHOD-2"
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
        ??? success "Output"
            ```
            36
            All Divisors are: 1 36 2 18 3 12 4 9 6
            ```