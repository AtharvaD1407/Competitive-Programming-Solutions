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

<hr>

# Java
```java
import java.util.Scanner;

public class TeamCount {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int n = scanner.nextInt();
        scanner.nextLine();
        int count = 0;

        for (int i = 0; i < n; i++) {
            String[] parts = scanner.nextLine().split(" ");
            int sum = 0;
            for (String part : parts) {
                sum += Integer.parseInt(part);
            }
            if (sum >= 2) {
                count++;
            }
        }

        System.out.println(count);
        scanner.close();
    }
}
```
