---
icon: material/numeric-4-box-multiple
---

!!! example "Example"
    === "C++"
        ???+ tip "print_Nto1.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void print_Nto1(int n){
                if(n==0)
                    return;
                cout << n << " ";
                print_Nto1(n-1);
            }

            int main() {
                int n;
                cin >> n;
                print_Nto1(n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5
            5 4 3 2 1
            ```