---
icon: material/numeric-4-circle
---

``` mermaid
graph LR
  A(Start) --> B[Expression];
  B --> C1{Case 1};
  C1 --> |Match| S1[Statement 1];
  S1 --> B1[break];
  B1 --> I[End];
  C1 --> |Unmached| C2{Case 2};
  C2 --> |Match| S2[Statement 2];
  S2 --> B2[break];
  B2 --> I[End];
  C2 --> |Unmached| C3{Case 3};
  C3 --> |Match| S3[Statement 3];
  S3 --> B3[break];
  B3 --> I[End];
  C3 --> |Unmached| Cn{Case n};
  Cn --> |Match| Sn[Statement n];
  Sn --> Bn[break];
  Bn --> I[End];
  Cn --> |Unmached| De[Default];
  De --> Sd[Default Statement];
  Sd --> Bd[break];
  Bd --> I[End];

  style A fill:#f00,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
  style I fill:#00f,color:white,font-weight:bold,stroke-width:2px,stroke:yellow

  subgraph Switch_Number
    B[Switch Number]
  end

  subgraph Case_1
    C1{Case 1}
  end

  subgraph Case_2
    C2{Case 2}
  end

  subgraph Case_3
    C3{Case 3}
  end

  subgraph Case_n
    Cn{Case n}
  end

  subgraph Default
    De{Default}
  end

  subgraph Statement_Group_1
    S1[Statement Group 1]
  end

  subgraph Statement_Group_2
    S2[Statement Group 2]
  end

  subgraph Statement_Group_3
    S3[Statement Group 3]
  end

  subgraph Statement_Group_n
    Sn[Statement Group n]
  end

  subgraph Default_Statement_Group
    Sd[Default Statement Group]
  end

  style Switch_Number fill:##FC33FF,stroke:#FF6E40,stroke-width:5px;
  style Case_1 fill:##FC33FF,stroke:#3A9D23,stroke-width:5px;
  style Case_2 fill:##FC33FF,stroke:#3A9D23,stroke-width:5px;
  style Case_3 fill:##FC33FF,stroke:#3A9D23,stroke-width:5px;
  style Case_n fill:##FC33FF,stroke:#3A9D23,stroke-width:5px;
  style Default fill:##FC33FF,stroke:#3A9D23,stroke-width:5px;
  style Statement_Group_1 fill:##FC33FF,stroke:#4D5BFF,stroke-width:5px;
  style Statement_Group_2 fill:##FC33FF,stroke:#4D5BFF,stroke-width:5px;
  style Statement_Group_3 fill:##FC33FF,stroke:#4D5BFF,stroke-width:5px;
  style Statement_Group_n fill:##FC33FF,stroke:#4D5BFF,stroke-width:5px;
  style Default_Statement_Group fill:##FC33FF,stroke:#4D5BFF,stroke-width:5px;

```


!!! example
    !!! question "Problem"
        ```cpp
        Take the day number and print the corresponding day
        for 1 print Monday
        for 2 print Tuesday and so on for 7 print Sunday           
        ```
    === "C++"
        !!! tip "Switch.cpp"
            ```cpp linenums="1" hl_lines="8-31"
            #include <bits/stdc++.h>
            using namespace std;

            int main() {
                int day;
                cin >> day;

                switch(day) {
                    case 1:
                        cout << "Monday";
                        break;
                    case 2:
                        cout << "Tuesday";
                        break;
                    case 3:
                        cout << "Wednesday";
                        break;
                    case 4:
                        cout << "Thursday";
                        break;
                    case 5:
                        cout << "Friday";
                        break;
                    case 6:
                        cout << "Saturday";
                        break;
                    case 7:
                        cout << "Sunday";
                        break;
                    default:
                        cout << "Invalid";
                }
                cout << " Check";
                return 0;
            }
            ```
        ??? success "Output"
            ```
            4
            Thursday Check
            ```
        ??? success "Output"
            ```
            8
            Invalid Check
            ```