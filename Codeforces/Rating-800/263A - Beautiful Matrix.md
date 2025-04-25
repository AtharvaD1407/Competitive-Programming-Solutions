# Python
```python
rowNo, colNo = 0, 0

for i in range(1, 6):
    row = list(map(int, input().split()))
    if 1 in row:
        rowNo = i
        colNo = row.index(1) + 1
        break

moves = abs(rowNo - 3) + abs(colNo - 3)

print(moves)
```

<hr>

# C++
```c++
#include <iostream>
#include <cmath>

using namespace std;

int main() {
    int rowNo = 0, colNo = 0;
    int val;

    for (int i = 1; i <= 5; ++i) {
        for (int j = 1; j <= 5; ++j) {
            cin >> val;
            if (val == 1) {
                rowNo = i;
                colNo = j;
            }
        }
    }

    int moves = abs(rowNo - 3) + abs(colNo - 3);
    cout << moves << endl;

    return 0;
}
```

<hr>

# Java
```java
import java.util.Scanner;

public class BeautifulMatrix {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int rowNo = 0, colNo = 0;

        for (int i = 1; i <= 5; i++) {
            for (int j = 1; j <= 5; j++) {
                int value = scanner.nextInt();
                if (value == 1) {
                    rowNo = i;
                    colNo = j;
                }
            }
        }

        int moves = Math.abs(rowNo - 3) + Math.abs(colNo - 3);
        System.out.println(moves);

        scanner.close();
    }
}
```
