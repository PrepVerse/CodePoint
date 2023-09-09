---
icon: material/numeric-7-box
---

## METHOD-1
!!! example "Example"
    === "C++"
        ???+ tip "check_Prime.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            string check_Prime(int n){
                for (int i = 2; i < n; i++) {
                    if (n % i == 0) {
                        return "false";
                    }
                }
                return "true";
            }

            int main() {
                int n;
                cin >> n;
                cout << check_Prime(n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            36
            false
            ```

## METHOD-2
!!! example "Example"
    === "C++"
        ???+ tip "check_Prime.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            string check_Prime(int n){
                for (int i = 2; i < sqrt(n); i++) {
                    if (n % i == 0) {
                        return "false";
                    }
                }
                return "true";
            }

            int main() {
                int n;
                cin >> n;
                cout << check_Prime(n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            36
            false
            ```