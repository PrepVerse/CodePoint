---
icon: material/numeric-2-box
---

!!! example ""
    === "C++"
        ???+ tip "ReverseNumber.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            int ReverseNumber(int n){
                int reverse_Num = 0;
                while(n > 0) {
                    int digit = n%10;
                    reverse_Num = reverse_Num*10 + digit;
                    n /= 10;
                }
                return reverse_Num;
            }

            int main() {
                int n;
                cin >> n;
                cout << ReverseNumber(n);
                return 0;
            }
            ```
            /// html | div.result
            ++'Input'++: 5432 <br>
            ++'Output'++: 2345
            ///