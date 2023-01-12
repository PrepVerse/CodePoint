!!! example "Example"
    === "C++"
        ???+ tip "print_1toN.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void print_1toN(int n){
                if(n==0)
                    return;
                print_1toN(n-1);
                cout << n << " ";
            }

            int main() {
                int n;
                cin >> n;
                print_1toN(n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5
            1 2 3 4 5
            ```