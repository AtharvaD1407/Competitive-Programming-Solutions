# Python
```python
n = int(input())
count = 0

for _ in range(n):
    if sum(map(int, input().split())) >= 2:
        count += 1

print(count)
```

<hr>

# C++
```c++
#include <iostream>
#include <string>
using namespace std;

int main()
{
    int n, x = 0;
    cin >> n;
    cin.ignore();

    for (int i = 0; i < n; i++)
    {
        string operation;
        getline(cin, operation);

        x += (operation.find('+') != string::npos) ? 1 : -1;
    }

    cout << x << endl;

    return 0;
}
```
