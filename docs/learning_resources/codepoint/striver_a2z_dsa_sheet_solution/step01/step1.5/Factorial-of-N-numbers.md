!!! example "Example"
    === "C++"
        ???+ tip "factorialOf_N_Numbers.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            int factorialOf_N_Numbers(int n){
                int fact = 1;
                if(n==0)
                    return 1;
                fact = n * factorialOf_N_Numbers(n-1);
                return fact;
            }

            int main() {
                int n;
                cin >> n;
                cout << factorialOf_N_Numbers(n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5
            120
            ```