---
icon: material/numeric-6-circle
---

``` mermaid
graph LR

  A(Start) --> B[Initialize Variables];
  B --> C{Condition};
  C --> |True| D[Execute Loop Body];
  D --> E[Update Variables];
  E --> C;
  C --> |False| F(End);

  style A fill:#f00,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
  style F fill:#00f,color:white,font-weight:bold,stroke-width:2px,stroke:yellow

  subgraph Initialize_Variables
    B[Initialization]
  end

  subgraph Condition
    C{Condition}
  end

  subgraph Execute_Loop_Body
    D[Loop Body]
  end

  subgraph Update_Variables
    E[Update]
  end

  style Initialize_Variables fill:##FC33FF,stroke:#FF6E40,stroke-width:5px;
  style Condition fill:##FC33FF,stroke:#F6fE40,stroke-width:5px;
  style Execute_Loop_Body fill:##FC33FF,stroke:#3A9D23,stroke-width:5px;
  style Update_Variables fill:##FC33FF,stroke:#4D5BFF,stroke-width:5px;

```


!!! example ""
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
            /// html | div.result
            ++'Output'++: 55
            ///

