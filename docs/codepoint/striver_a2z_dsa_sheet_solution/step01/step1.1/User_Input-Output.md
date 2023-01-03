``` mermaid
graph LR
  A(Start) --> B[Declare Variable n1, n2 & Sum];
  B ----> C[Read n1 & n2];
  C --> D[Sum <-- n1+n2];
  D --> E[Display Sum];
  E --> F(End);
```


!!! example
    === "C"
        !!! question "Sum of 2 Numbers.c"
            ```c linenums="1" hl_lines="4-13"
            #include <stdio.h>

            int main() {    
                int number1, number2, sum;
                
                printf("Enter two integers: ");
                scanf("%d %d", &number1, &number2);

                // calculating sum
                sum = number1 + number2;      
                
                // prints sum 
                printf("%d + %d = %d", number1, number2, sum);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            Enter two integers: 12 
            11
            12 + 11 = 23
            ```
    === "C++"
        !!! question "Sum of 2 Numbers.cpp"
            ```cpp linenums="1" hl_lines="5-14"
            #include <iostream>
            using namespace std;

            int main() {
                int number1, number2, sum;
                
                cout << "Enter two integers: ";
                cin >> number1 >> number2;

                // calculating sum
                sum = number1 + number2;

                // prints sum 
                cout << number1 << " + " <<  number2 << " = " << sum;     
                return 0;
            }
            ```
        ??? success "Output"
            ```
            Enter two integers: 12 
            11
            12 + 11 = 23
            ```
    === "Java"
        !!! question "Sum of 2 Numbers.java"
            ```java linenums="1" hl_lines="5-17"
            import java.util.*;

            class Main {
                public static void main(String[] args) {
                    int number1, number2, sum;
                    Scanner scanner;
    
                    scanner = new Scanner(System.in);
                    System.out.println("Enter two integers: ");
                    number1 = scanner.nextInt();
                    number2 = scanner.nextInt();

                    // calculating sum
                    int sum = number1 + number2;

                    // prints sum
                    System.out.println(number1 + " + " + number2 + " = "  + sum);
                }
            }
            ```
        ??? success "Output"
            ```
            Enter two integers: 12 
            11
            12 + 11 = 23
            ```
    === "Python"
        !!! question "Sum of 2 Numbers.py"
            ```py linenums="1" hl_lines="1-8"
            print("Enter two integers: ")
            number1, number2 = int(input()), int(input())

            # calculating sum
            sum = number1 + number2

            # prints sum
            print(number1, "+", number2, "=", number1+number2)
            ```
        ??? success "Output"
            ```
            Enter two integers: 12 
            11
            12 + 11 = 23
            ```
            