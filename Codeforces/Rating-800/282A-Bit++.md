# Python
```python
n = int(input())
x = 0

for _ in range(n):
    x += 1 if "+" in input() else -1

print(x)
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

public class BitPlusPlus {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        int n = scanner.nextInt();
        scanner.nextLine(); // Consume newline
        int x = 0;

        for (int i = 0; i < n; i++) {
            String statement = scanner.nextLine();
            if (statement.contains("+")) {
                x += 1;
            } else {
                x -= 1;
            }
        }

        System.out.println(x);
        scanner.close();
    }
}
```
