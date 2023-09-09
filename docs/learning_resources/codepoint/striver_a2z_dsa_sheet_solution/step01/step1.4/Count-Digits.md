---
icon: material/numeric-1-box
---

## METHOD-1
!!! example "Example"
    === "C++"
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
## METHOD-2
!!! example "Example"
    === "C++"
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