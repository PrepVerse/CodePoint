---
icon: material/dots-triangle
---

# 17. Triangle Character Pattern

!!! example "Example"
    !!! question "Pattern 17"
        <h1 align="center">$N = 5$</h1>

        $$\Large
        \begin{align*}
            &\phantom{A}\phantom{A}\phantom{A}\phantom{A}A \\
            &\phantom{A}\phantom{A}\phantom{A}ABA \\
            &\phantom{A}\phantom{A}ABCBA \\
            &\phantom{A}ABCDCBA \\
            &ABCDEDCBA \\
        \end{align*}
        $$
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                for(int i=1; i<=n; i++) {
                    char ch = 'A';
                    for(int j=0; j<n-i; j++) {
                        cout << " ";
                    }
                    for(int j=0; j<i; j++) {
                        cout << ch++;
                    }
                    --ch;
                    for(int j=1; j<i; j++) {
                        cout << --ch;
                    }
                    cout << endl;
                }
            }

            int main(void) {
                int n;
                cin >> n;
                printTriangle(n);
                return 0;
            }
            ```
            /// html | div.result
            ++'Input'++: 5 <br>
            ++'Output'++:
            ```
                A
               ABA
              ABCBA
             ABCDCBA
            ABCDEDCBA
            ```