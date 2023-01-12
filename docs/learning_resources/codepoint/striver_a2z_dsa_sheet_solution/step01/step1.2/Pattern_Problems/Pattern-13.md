!!! example "Example"
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                int num=1;
                for(int i=1; i<=n; i++) {
                    for(int j=0; j<i; j++) {
                        cout << num++ << " ";
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
        ??? success "Output"
            ```
            5
            1 
            2 3 
            4 5 6 
            7 8 9 10 
            11 12 13 14 15
            ```