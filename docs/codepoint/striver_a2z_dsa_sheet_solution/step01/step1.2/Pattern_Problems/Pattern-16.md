!!! example "Example"
    === "C++"
        ???+ tip "printTriangle.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void printTriangle(int n) {
                char ch = 'A';
                for(int i=1; i<=n; i++) {
                    for(int j=0; j<i; j++) {
                        cout << ch;
                    }
                    ch++;
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
            A
            BB
            CCC
            DDDD
            EEEEE
            ```