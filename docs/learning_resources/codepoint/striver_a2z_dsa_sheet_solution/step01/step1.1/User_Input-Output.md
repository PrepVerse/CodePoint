---
icon: material/numeric-1-circle
---

``` mermaid
graph LR

  A(Start) --> B[Declare Variables];
  B --> C[Read User Input];
  C --> D[Process Input];
  D --> E[Generate Output];
  E --> F[Display Output to User];
  F --> G(End);

  style A fill:#f00,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
  style G fill:#00f,color:white,font-weight:bold,stroke-width:2px,stroke:yellow

  subgraph Declare_Variables
    B[Declare Variables]
  end

  subgraph Read_User_Input
    C[Read User Input]
  end

  subgraph Process_Input
    D[Process Input]
  end

  subgraph Generate_Output
    E[Generate Output]
  end

  subgraph Display_Output
    F[Display Output to User]
  end

  style Declare_Variables fill:##FC33FF,stroke:#FF6E40,stroke-width:4px;
  style Read_User_Input fill:##FC33FF,stroke:#3A9D23,stroke-width:4px;
  style Process_Input fill:##FC33FF,stroke:#4D5BFF,stroke-width:4px;
  style Generate_Output fill:##FC33FF,stroke:#FF406A,stroke-width:4px;
  style Display_Output fill:##FC33FF,stroke:#0082FF,stroke-width:4px;

```

!!! example ""
    ## Input
    === "C++"
        !!! abstract "User Input in C++"
            To read input from the user in C++, you can use the {==++'cin'++==} stream. Here's an example of how to read an integer from the user
        !!! tip "Input.cpp"
            ```cpp linenums="1" hl_lines="5-6"
            #include <bits/stdc++.h>
            using namespace std;

            int main() {
                int x, y;
                cin >> x >> y;
                cout << "Value of x=" << x << " and y=" << y;
                return 0;
            }
            ```
            /// html | div.result
            ++'Input'++: 10 11 <br>
            ++'Output'++: Value of x=10 and y=11
            ///
    === "Python"
        !!! abstract "User Input in Python"
            To read input from the user in Python, you can use the {==++'input()'++==} function. Here's an example of how to read a integer from the user
        !!! tip "Input.py"
            ```py linenums="1" hl_lines="1-2"
            x, y = list(map(int, input().split()))
            print("Value of x=", x, "and y=", y)
            ```
            /// html | div.result
            ++'Input'++: 10 11 <br>
            ++'Output'++: Value of x=10 and y=11
            ///
    ## Output
    === "C++"
        !!! abstract "User Output in C++"
            To display output to the user in C++, you can use the {==++'cout'++==} stream. Here's an example of how to output a message to the user
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
            /// html | div.result
            ++'Output'++: Hello, <br> My Name is Akash Singh
            ///
    === "Python"
        !!! abstract "User Output in Python"
            To display output to the user in Python, you can use the {==++'print()'++==} function. Here's an example of how to output a message to the user
        !!! tip "Output.py"
            ```py linenums="1" hl_lines="1-2"
            print("Hello,")
            print("My Name is", "Akash Singh")
            ```
            /// html | div.result
            ++'Output'++: Hello, <br> My Name is Akash Singh
            ///
