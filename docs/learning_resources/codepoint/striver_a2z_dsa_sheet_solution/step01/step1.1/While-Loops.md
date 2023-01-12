# While Loops
``` mermaid
graph LR
  A[Start] --> B{Condition};
  B ---->|True| E[Statement];
  E[Statement] --> A[Start];
  B -->|False| C[End];
```
# Do-While Loops
``` mermaid
graph LR
  A[Start] --> B[Do];
  B--> C[Condition];
  C --> D{While Condition};
  D -->|True| C[Condition];
  D -->|False| E[End];
```


!!! example
    === "C++ : WHILE"
        !!! tip "Sum of 10 Numbers.cpp"
            ```c++ linenums="1" hl_lines="6-10"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                int sum=0;
                int n=1;
                while(n <= 10) {
                    sum += n;
                    n++;
                }  
                cout << sum;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            55
            ```
    === "C++ : DO - WHILE"
        !!! tip "Sum of 10 Numbers.cpp"
            ```c++ linenums="1" hl_lines="6-10"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                int sum=0;
                int n=1;
                do {
                    sum += n;
                    n++;
                } while(n <= 10);
                cout << sum;
                return 0;
            }
            ```
        ??? success "Output"
            ```
            55
            ```

