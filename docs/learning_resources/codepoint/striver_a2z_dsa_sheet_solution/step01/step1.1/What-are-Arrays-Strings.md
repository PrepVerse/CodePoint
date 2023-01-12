!!! example
    === "C++ : Array _ METHOD-1"
        !!! tip "Array.cpp"
            ```c++ linenums="1" hl_lines="5-9"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                int a, b, c, d, e
                cin >> a >> b >> c >> d >> e;

                int sum = a + b + c + d + e;
                cout << sum;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            1 2 3 4 5
            15
            ```
    === "C++ : Array _ METHOD-2"
        !!! tip "Array.cpp"
            ```c++ linenums="1" hl_lines="5-9"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                int arr[5];
                cin >> arr[0] >> arr[1] >> arr[2] >> arr[3] >> arr[4];

                int sum = arr[0] + arr[1] + arr[2] + arr[3] + arr[4];
                cout << sum;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            1 2 3 4 5
            15
            ```
    === "C++ : 2D Array _ METHOD-1"
        !!! tip "Matrix.cpp"
            ```c++ linenums="1" hl_lines="5-9"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                int arr[2][2];
                cin >> arr[0][0] >> arr[0][1] >> arr[1][0] >> arr[1][1];

                int sum = arr[0][0] + arr[0][1] + arr[1][0] + arr[1][1];
                cout << sum;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            1 2 3 4
            10
            ```
    === "C++ : String _ METHOD-1"
        !!! tip "String.cpp"
            ```c++ linenums="1" hl_lines="5-7"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                string str = "Akash Singh";
                int len = str.size();
                cout << str[len-1];
                return 0;
            }
            ```
        ??? success "Output"
            ```
            h
            ```

