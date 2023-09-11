---
icon: material/numeric-5-box-multiple
---

!!! example ""
    === "C++"
        ???+ tip "sumOf_N_Numbers.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            int sumOf_N_Numbers(int n){
                int sum=0;
                if(n==0)
                    return 0;
                sum = n + sumOf_N_Numbers(n-1);
                return sum;
            }

            int main() {
                int n;
                cin >> n;
                cout << sumOf_N_Numbers(n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5
            15
            ```