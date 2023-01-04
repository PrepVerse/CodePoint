``` mermaid
graph LR
  A[Start] --> B{Last Item?};
  B -->|No| E[Statement];
  E[Statement] -->|Try Next Number| A[Start];
  B -->|Yes| C[End];
```


!!! example
    === "C++"
        !!! tip "Sum of 10 Numbers.cpp"
            ```c++ linenums="1" hl_lines="6-8"
            #include<bits/stdc++.h>
            using namespace std;

            int main() {
                int sum=0;
                for(int i=1; i<=10; i++) {
                    sum += i;
                }   
                cout << sum;
            }
            ```
        ??? success "Output"
            ```
            55
            ```

