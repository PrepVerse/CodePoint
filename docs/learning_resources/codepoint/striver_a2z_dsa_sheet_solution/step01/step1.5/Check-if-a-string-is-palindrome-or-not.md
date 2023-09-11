---
icon: material/numeric-8-box-multiple
---

!!! example ""
    === "C++"
        ???+ tip "check_Palindrome.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            string check_Palindrome(string str, int start, int end){
                if(end - start == 1 or start == end) {
                    return "true";
                }
                else if(str[start] == str[end]) {
                    return check_Palindrome(str, start+1, end-1);
                }
                else {
                    return "false";
                }
            }

            int main() {
                string str;
                cin >> str;
                int n = str.size();
                cout << check_Palindrome(str, 0, n-1);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            ABCDCBA
            true
            ```