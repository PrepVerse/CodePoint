!!! example "Example"
    === "C++ : METHOD-1"
        ???+ tip "countDigits.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            int countDigits(int n){
                int count = 0;
                while(n > 0) {
                    n /= 10;
                    count++;
                }
                return count;
            }

            int main() {
                int n;
                cin >> n;
                cout << countDigits(n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5432
            4
            ```
    === "C++ : METHOD-2"
        ???+ tip "countDigits.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            int countDigits(int n){
                int count = floor(log10(n) + 1);
                return count;
            }

            int main() {
                int n;
                cin >> n;
                cout << countDigits(n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5432
            4
            ```