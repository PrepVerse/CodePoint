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
        ```c linenums="1" hl_lines="4-13" title="Sum of 2 Numbers.c"
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
        ```title="Output"
        Enter two integers: 12 
        11
        12 + 11 = 23
        ```
    === "C++"
        ```cpp linenums="1" hl_lines="5-14" title="Sum of 2 Numbers.cpp"
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
        ```title="Output"
        Enter two integers: 12 
        11
        12 + 11 = 23
        ```
    === "Java"
        ```java linenums="1" hl_lines="5-17" title="Sum of 2 Numbers.cpp"
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
        ```title="Output"
        Enter two integers: 12 
        11
        12 + 11 = 23
        ```
    === "Python"
        ```py linenums="1" hl_lines="1-8" title="Sum of 2 Numbers.py"
        print("Enter two integers: ")
        number1, number2 = int(input()), int(input())

        # calculating sum
        sum = number1 + number2

        # prints sum
        print(number1, "+", number2, "=", number1+number2)
        ```
        ```title="Output"
        Enter two integers: 12 
        11
        12 + 11 = 23
        ```
        