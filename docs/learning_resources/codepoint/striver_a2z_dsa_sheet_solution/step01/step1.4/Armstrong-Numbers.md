!!! example "Example"
    === "C++"
        ???+ tip "Armstrong_Num.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            string Armstrong_Num(int n){
                int Num = n;
                int armstrong_Num = 0;
                int len = floor(log10(n) + 1);
                while(n > 0) {
                    int digit = n%10;
                    armstrong_Num += pow(digit, len);
                    n /= 10;
                }
                return armstrong_Num == Num ? "true" : "false";
            }

            int main() {
                int n;
                cin >> n;
                cout << Armstrong_Num(n);
                return 0;
            }
            ```
        ??? success "Output"
            ``` yaml
            1634 # (1)!
            true
            ```

            1.  $1^4 + 6^4 + 3^4 + 4^4 = 1634$