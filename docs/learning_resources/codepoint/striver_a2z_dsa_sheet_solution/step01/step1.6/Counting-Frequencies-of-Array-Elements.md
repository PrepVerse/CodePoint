!!! example "Example"
    === "C++ : METHOD-1"
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
                    int count = 1;
                    for (int j = i + 1; j < n; j++) {
                        if (arr[i] == arr[j]) {
                            visited[j] = true;
                            count++;
                        }
                    }
                    cout << arr[i] << " " << count << endl;
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
            10 3
            2 2
            4 1
            ```
    === "C++ : METHOD-2"
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
            10 3
            2 2
            4 1
            ```