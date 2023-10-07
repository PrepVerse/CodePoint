---
icon: material/numeric-3-box
---

!!! example ""
    === "C++"
        ???+ tip "check_Palindrome.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            string check_Palindrome(int n){
                int Num = n;
                int reverse_Num = 0;
                while(n > 0) {
                    int digit = n%10;
                    reverse_Num = reverse_Num*10 + digit;
                    n /= 10;
                }
                return reverse_Num == Num ? "true" : "false";
            }

            int main() {
                int n;
                cin >> n;
                cout << check_Palindrome(n);
                return 0;
            }
            ```
            /// html | div.result
            ++'Input'++: 1331 <br>
            ++'Output'++: true
            ///