---
icon: material/numeric-4-box
---

!!! example ""
    ## Method-1
    === "C++"
        ???+ tip "find_GCD-LCM.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            int GCD(int a, int b){
                int gcd = 0;
                for (int i = 1; i <= min(a, b); i++) {
		            if (a % i == 0 and b % i == 0) {
			            gcd = i;
                    }
                }
                return gcd;
            }

            int LCM(int a, int b){
                int gcd = GCD(a, b);
                int lcm = (a*b)/gcd;
                return lcm;
            }

            int main() {
                int a, b;
                cin >> a >> b;
                cout << "GCD: " << GCD(a, b) << endl;
                cout << "LCM: " << LCM(a, b) << endl;
                return 0;
            }
            ```
            /// html | div.result
            ++'Input'++: 5 10 <br>
            ++'Output'++: GCD: 5 <br> LCM: 10
            ///
    ## Method-2
    === "C++"
        ???+ tip "find_GCD-LCM.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            int GCD(int a, int b){
                if (b == 0) {
		            return a;
                }
                return GCD(b, a % b);
            }

            int LCM(int a, int b){
                int gcd = GCD(a, b);
                int lcm = (a*b)/gcd;
                return lcm;
            }

            int main() {
                int a, b;
                cin >> a >> b;
                cout << "GCD: " << GCD(a, b) << endl;
                cout << "LCM: " << LCM(a, b) << endl;
                return 0;
            }
            ```
            /// html | div.result
            ++'Input'++: 5 10 <br>
            ++'Output'++: GCD: 5 <br> LCM: 10
            ///