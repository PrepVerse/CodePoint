``` mermaid
graph LR
  A(Start) --> B[Switch Number];
  B --> C{Case 1};
  C --> D{Case 2};
  D --> E{Case n};
  C --> |Yes| F[Statemet Group 1];
  D --> |Yes| G[Statemet Group 2];
  E --> |Default| H[Statemet Group n];
  F --> |Break Statement| I[End];
  G --> |Break Statement| I[End];
  H --> |Break Statement| I[End];
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