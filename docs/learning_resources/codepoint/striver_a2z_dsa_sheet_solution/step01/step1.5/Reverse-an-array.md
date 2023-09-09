---
icon: material/numeric-7-box-multiple
---

!!! example "Example"
    === "C++"
        ???+ tip "reverse_Array.cpp"
            ``` c++ linenums="1"
            #include <bits/stdc++.h>
            using namespace std;

            void reverse_Array(int arr[], int start, int end){
                if(start < end) {
                    swap(arr[start], arr[end]);
                    reverse_Array(arr, start+1, end-1);
                }
            }

            int main() {
                int n;
                cin >> n;
                int arr[n];
                for(int i=0; i<n; i++) {
                    cin >> arr[i];
                }
                reverse_Array(arr, 0, n-1);
                for(int i=0; i<n; i++) {
                    cout << arr[i] << " ";
                }
                return 0;
            }
            ```
        ??? success "Output"
            ```
            5
            1 2 3 4 5
            5 4 3 2 1
            ```