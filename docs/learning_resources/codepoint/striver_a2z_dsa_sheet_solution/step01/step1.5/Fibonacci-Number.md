---
icon: material/numeric-9-box-multiple
---

!!! example ""
    === "C++"
        ???+ tip "fibonacci.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            int fibonacci(int n){
                if(n == 0 or n == 1)
                    return n;
                int fibb = fibonacci(n-1) + fibonacci(n-2);
                return fibb;
            }

            int main() {
                int n;
                cin >> n;
                for(int i=0; i<n; i++)
                    cout << fibonacci(i) <<" ";
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5
            0 1 1 2 3
            ```