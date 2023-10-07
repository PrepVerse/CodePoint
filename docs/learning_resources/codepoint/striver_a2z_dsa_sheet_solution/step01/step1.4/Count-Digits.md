---
icon: material/numeric-1-box
---

!!! example ""
    ## Method-1
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
            /// html | div.result
            ++'Input'++: 5432 <br>
            ++'Output'++: 4
            ///
    ## Method-2
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
            /// html | div.result
            ++'Input'++: 5432 <br>
            ++'Output'++: 4
            ///