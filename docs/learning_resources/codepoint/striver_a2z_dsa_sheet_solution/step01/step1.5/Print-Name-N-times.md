!!! example "Example"
    === "C++"
        ???+ tip "print_Name.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void print_Name(int n){
                if(n==0)
                    return;
                cout << "Akash Singh" << endl;
                print_Name(n-1);
            }

            int main() {
                int n;
                cin >> n;
                print_Name(n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5
            Akash Singh
            Akash Singh
            Akash Singh
            Akash Singh
            Akash Singh
            ```