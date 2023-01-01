``` mermaid
graph LR
  A[Start] --> B{Last Item?};
  B ---->|No| E[Statement];
  E[Statement] -->|Try Next Number| A[Start];
  B -->|Yes| C[End];
```


!!! example
    === "C++"
        ```c++ linenums="1" hl_lines="3-5" title="Sum of 10 Numbers.cpp"
        int main() {
            int sum=0;
            for(int i=1; i<10; i++) {
                sum += i;
            }   
            cout << sum;
        }
        ```

