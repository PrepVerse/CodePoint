``` mermaid
graph LR
  A(Start) --> B[Declare Variables];
  B --> C[Read variables];
  C --> D[Display Result];
  D --> E(End);
```


!!! example
    === "C++ : OUTPUT"
        !!! tip "Output.cpp"
            ```cpp linenums="1" hl_lines="5-6"
            #include <bits/stdc++.h>
            using namespace std;

            int main() {
                cout << "Hello," << endl;
                cout << "My Name is " << "Akash Singh" << endl;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            Hello,
            My Name is Akash Singh
            ```

    === "C++ : INPUT"
        !!! tip "Input.cpp"
            ```cpp linenums="1" hl_lines="5-6"
            #include <bits/stdc++.h>
            using namespace std;

            int main() {
                int x, y;
                cin >> x >> y;
                cout << "Value of x: " << x << " and y: " << y;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            10 11
            Value of x: 10 and y: 11
            ```