---
icon: octicons/hash-16
---

## METHOD-1
!!! example "Example"
    === "C++"
        ???+ tip "count_Frequency.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void count_Frequency(int arr[], int n){
                vector<bool> visited(n, false);
                for (int i = 0; i < n; i++) {
                    if (visited[i] == true) {
                        continue;
                    }
                    int count = 1, max_count=0;
                    for (int j = i + 1; j < n; j++) {
                        if (arr[i] == arr[j]) {
                            visited[j] = true;
                            count++;
                        }
                    }
                    if (count > maxcount) {
                        max_count = count;
                    }
                    cout << "Heighest Frequency = " << max_count;
                }
            }

            int main() {
                int n;
                cin >> n;
                int arr[n];
                for(int i=0; i<n; i++) {
                    cin >> arr[i];
                }
                count_Frequency(arr, n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            6
            10 2 10 4 10 2
            Heighest Frequency = 3
            Lowest Frequency = 1
            ```

## METHOD-2
!!! example "Example"
    === "C++"
        ???+ tip "count_Frequency.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void count_Frequency(int arr[], int n){
                unordered_map<int, int> map;
                for (int i = 0; i < n; i++) {
                    map[arr[i]]++;
                }
                for (auto x : map) {
                    cout << x.first << " " << x.second << endl;
                }
                int max_count = 0, res = -1; 
                for (auto i : map) { 
                    if (max_count < i.second) { 
                        res = i.first; 
                        max_count = i.second; 
                    } 
                }
                cout << "Heighest Frequency = " << max_count;
            }

            int main() {
                int n;
                cin >> n;
                int arr[n];
                for(int i=0; i<n; i++) {
                    cin >> arr[i];
                }
                count_Frequency(arr, n);
                return 0;
            }
            ```
        ??? success "Output"
            ```
            6
            10 2 10 4 10 2
            Heighest Frequency = 3
            Lowest Frequency = 1
            ```