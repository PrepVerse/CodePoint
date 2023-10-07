---
icon: material/numeric-7-circle
---

!!! abstract "While Loops"
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

      subgraph Loop_Condition
        C{Condition}
      end

      subgraph Execute_Loop_Body
        D[Loop Body]
      end

      subgraph Update_Variables
        E[Update]
      end

      style Initialize_Variables fill:##FC33FF,stroke:#FF6E40,stroke-width:5px;
      style Loop_Condition fill:##FC33FF,stroke:#3A9D23,stroke-width:5px;
      style Execute_Loop_Body fill:##FC33FF,stroke:#4D5BFF,stroke-width:5px;
      style Update_Variables fill:##FC33FF,stroke:#FF406A,stroke-width:5px;
    ```

!!! abstract "Do-While Loops"
    ```mermaid
    graph LR

      A(Start) --> B[Initialize Variables];
      B --> C(Loop Start);
      C --> D{Condition};
      D --> |True| E[Execute Loop Body];
      E --> F(End Loop);
      F --> G{Continue Loop?};
      G --> |True| D;
      G --> |False| H(End);

      style A fill:#f00,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
      style H fill:#00f,color:white,font-weight:bold,stroke-width:2px,stroke:yellow

      subgraph Initialize_Variables
        B[Variables]
      end

      subgraph Loop_Start
        C(Do)
      end

      subgraph Condition
        D{Condition}
      end

      subgraph Execute_Loop_Body
        E[Execute Do Body]
      end

      subgraph End_Loop
        F(Do Loop)
      end

      subgraph Continue_Loop
        G{Continue Loop?}
      end

      style Initialize_Variables fill:##FC33FF,stroke:#FF6E40,stroke-width:5px;
      style Loop_Start fill:##FC33FF,stroke:#3A9D23,stroke-width:5px;
      style Condition fill:##FC33FF,stroke:#3A9D23,stroke-width:5px;
      style Execute_Loop_Body fill:##FC33FF,stroke:#4D5BFF,stroke-width:5px;
      style End_Loop fill:##FC33FF,stroke:#FF406A,stroke-width:5px;
      style Continue_Loop fill:##FC33FF,stroke:#4D5BFF,stroke-width:5px;

    ```


!!! example ""
    ## While
    === "C++"
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
            /// html | div.result
            ++'Output'++: 55
            ///
    ## Do-While
    === "C++"
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
            /// html | div.result
            ++'Output'++: 55
            ///

