``` mermaid
graph LR

  A(Start) --> B[Initialize Variables];
  B --> C{Condition};
  C -- Yes --> D[Execute If Block];
  C -- No --> E[Execute Else Block];
  D --> F[Display Result];
  E --> F;
  F --> G(End);

  style A fill:#f00,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
  style G fill:#00f,color:white,font-weight:bold,stroke-width:2px,stroke:yellow

  subgraph Initialize_Variables
    B[Variables]
  end

  subgraph Condition
    C{Condition}
  end

  subgraph Execute_If_Block
    D[Execute If Block]
  end

  subgraph Execute_Else_Block
    E[Execute Else Block]
  end

  subgraph Display_Result
    F[Display Result]
  end

  style Initialize_Variables fill:##FC33FF,stroke:#FF6E40,stroke-width:5px;
  style Condition fill:##FC33FF,stroke:#045F7F,stroke-width:5px;
  style Execute_If_Block fill:##FC33FF,stroke:#3A9D23,stroke-width:5px;
  style Execute_Else_Block fill:##FC33FF,stroke:#4D5BFF,stroke-width:5px;
  style Display_Result fill:##FC33FF,stroke:#FF406A,stroke-width:5px;

```


!!! example
    !!! question "Problem"
        ```cpp
        Take the age from user and then decide accordingly
        1.  if age < 18.
            print --> You are not eligible for job.
        2.  if age >= 18 and age <= 54.
            print --> You are eligible for job.
        3.  if age >= 55 and age <= 57.
            print --> You are eligible for job, but retirement soon.
        4.  if age > 57.
            print --> Retirement time.            
        ```
    === "C++ : METHOD-1"
        !!! tip "If_Else.cpp"
            ```cpp linenums="1" hl_lines="8-19"
            #include <bits/stdc++.h>
            using namespace std;

            int main() {
                int age;
                cin >> age;

                if(age < 18) {
                    cout << "You are not eligible for job.";
                }
                if(age >= 18 and age <= 54) {
                    cout << "You are eligible for job.";
                }
                if(age >= 55 and age <= 57) {
                    cout << "You are eligible for job, but retirement soon.";
                }
                if(age > 57) {
                    cout << "Retirement time.";
                }
                return 0;
            }
            ```
        ??? success "Output"
            ```
            22
            You are eligible for job.
            ```
    === "C++ : METHOD-2"
        !!! tip "If_Else.cpp"
            ```cpp linenums="1" hl_lines="8-19"
            #include <bits/stdc++.h>
            using namespace std;

            int main() {
                int age;
                cin >> age;
                
                if(age < 18) {
                    cout << "You are not eligible for job.";
                }
                else if(age <= 54) {
                    cout << "You are eligible for job.";
                }
                else if(age <= 57) {
                    cout << "You are eligible for job, but retirement soon.";
                }
                else if(age > 57) {
                    cout << "Retirement time.";
                }
                return 0;
            }
            ```
        ??? success "Output"
            ```
            22
            You are eligible for job.
            ```
    === "C++ : METHOD-3"
        !!! tip "If_Else.cpp"
            ```cpp linenums="1" hl_lines="8-19"
            #include <bits/stdc++.h>
            using namespace std;

            int main() {
                int age;
                cin >> age;
                
                if(age < 18) {
                    cout << "You are not eligible for job.";
                }
                else if(age <= 54) {
                    cout << "You are eligible for job.";
                }
                else if(age <= 57) {
                    cout << "You are eligible for job, but retirement soon.";
                }
                else {
                    cout << "Retirement time.";
                }
                return 0;
            }
            ```
        ??? success "Output"
            ```
            22
            You are eligible for job.
            ```
    === "C++ : METHOD-4"
        !!! tip "If_Else.cpp"
            ```cpp linenums="1" hl_lines="8-19"
            #include <bits/stdc++.h>
            using namespace std;

            int main() {
                int age;
                cin >> age;
                
                if(age < 18) {
                    cout << "You are not eligible for job.";
                }
                else if(age <= 57) {
                    cout << "You are eligible for job";
                    if(age >= 55) {
                        cout << ", but retirement soon.";
                    }
                }
                else {
                    cout << "Retirement time.";
                }
                return 0;
            }
            ```
        ??? success "Output"
            ```
            22
            You are eligible for job.
            ```
