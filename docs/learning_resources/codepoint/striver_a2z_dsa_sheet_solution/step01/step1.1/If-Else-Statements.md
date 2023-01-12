``` mermaid
graph LR
  A(Start) --> B[Expression];
  B --> |True| C[statement in if branch];
  B --> |False| D[statement in else branch];
  C --> E[End];
  D --> E(End);
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
