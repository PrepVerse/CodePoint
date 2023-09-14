!!! success ""
    ## 1. Find the Next One
    !!! tip ""
        ???+ question "Find the Next One"
            <h2> 
            **2, A, 9, B, 6, C, 13, D, ? (Infosys - 2019)**
            
            - [ ] 9
            - [X] 10
            - [ ] E
            - [ ] 15
        ??? abstract "Explanation"
            In this sequence, a number is followed by an alphabet and vice versa. Let's focus on the number pattern:
            ``` mermaid
            graph TD
                A[Start with 2] -->|Add 7| B[2 + 7 = 9]
                B -->|Subtract 3| C[9 - 3 = 6]
                C -->|Add 7| D[6 + 7 = 13]
                D -->|Subtract 3| E[13 - 3 = 10]
                E -->|Result| F[The next element in the sequence is: 10]
                    
                style A fill:#f00,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
                style F fill:#00f,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
            ```

    ## 2. Find the next alphanumeric code
    !!! success ""
        ???+ question "Find the next alphanumeric code"
            <h2>
            **2A11, 2D13, 4G17,? (IBM - 2017)**

            - [X] 12J23
            - [ ] 48M29
            - [ ] 36I29
            - [ ] 8E15
        ??? abstract "Explanation"
            ``` mermaid
            graph TD
                Start(2A11) -->|Multiply by 1| Step1(2D13)
                Step1 -->|Multiply by 2| Step2(4G17)
                Step2 -->|Multiply by 3| Result(12J23)
                Start -->|Move letter forward by 3| Step1
                Step1 -->|Move letter forward by 3| Step2
                Step2 -->|Move letter forward by 3| Result
                Start -->|Increase two digits by 2| Step1
                Step1 -->|Increase two digits by 4| Step2
                Step2 -->|Increase two digits by 6| Result
                    
                style Start fill:#f00,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
                style Result fill:#00f,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
            ```
            So, the next element in the sequence is: **12J23**

    ## 3. Find the missing value
    !!! info ""
        ???+ question "Find the missing value"
            <h2>
            **ACE, ?, MOQ, SUW(last term) (Wipro)**

            - [ ] GIL
            - [ ] EFH
            - [X] GIK
            - [ ] FHJ
        ??? abstract "Explanation"
            ``` mermaid
            graph TD
                Start(ACE) -->|Move letter forward by 6| Step1(GIK)
                Step1 -->|Move letter forward by 6| Step2(MOQ)
                Step2 -->|Move letter forward by | Result(SUW)
                Start -->|Move letter forward by 6| Step1
                Step1 -->|Move letter forward by 6| Step2
                Step2 -->|Move letter forward by 6| Result
                Start -->|Move letter forward by 6| Step1
                Step1 -->|Move letter forward by 6| Step2
                Step2 -->|Move letter forward by 6| Result
                    
                style Start fill:#f00,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
                style Step1 fill:#00f,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
            ```
            So, the next element in the sequence is: **GIK**

    ## 4. Lowest digit product
    !!! question ""
        ???+ question "Lowest digit product"
            <h2>
            **867 209 242 283 543  Given this series: <br> When the digits within the number are multiplied with each other, the product of which number is the lowest?**

            - [ ] 867
            - [X] 209
            - [ ] 242
            - [ ] 283
        ??? abstract "Explanation"
            ``` mermaid
            graph TD
                Start(867) -->|Multiply digits: 8 x 6 x 7| Step1(336)
                Start2(209) -->|Multiply digits: 2 x 0 x 9| Step3(0)
                Start3(242) -->|Multiply digits: 2 x 4 x 2| Step4(16)
                Start4(283) -->|Multiply digits: 2 x 8 x 3| Step5(48)
                Start5(543) -->|Multiply digits: 5 x 4 x 3| Step6(60)
                        
                style Start2 fill:#f00,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
                style Step3 fill:#00f,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
            ```

    ## 5. Find the character
    !!! danger ""
        ???+ question "Find the character"
            <h2>
            **Study the following arrangement carefully and answer the question that follows:**<br>
            **S K 6 & Q 2 R * C F 8 E $ G 2 # 4 9 L N 3 U V 5 Y α B 7 W 9**<br>
            **Which of the following letters, numbers, or symbols will be third to the left or a fifth of the left?**

            - [ ] Q
            - [ ] S
            - [X] 6
            - [ ] 2
        ??? abstract "Explanation"
            ``` mermaid
            graph TD
                Start(S K 6 & Q 2 R * C F 8 E $ G 2 # 4 9 L N 3 U V 5 Y α B 7 W 9) -->|Count 3 to the left| ThirdToLeft(6)
                ThirdToLeft -->|Count 5 of the left| FifthToLeft(R)
                ThirdToLeft -->|Check| Answer
                FifthToLeft -->|Check| Answer
                Answer -->|Display Result| Result(6)
                        
                style Start fill:#f00,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
                style Result fill:#00f,color:white,font-weight:bold,stroke-width:2px,stroke:yellow
            ```