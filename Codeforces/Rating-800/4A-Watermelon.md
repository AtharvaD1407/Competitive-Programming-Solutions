# Python
```python
w = int(input())

if w > 2 and w % 2 == 0:
    print("YES")
else:
    print("NO")
```

<hr>

# C++
```c++
#include <iostream>
using namespace std;

int main()
{

    int w;
    cin >> w;

    if (w > 2 && w % 2 == 0)
    {
        cout << "Yes" << endl;
    }
    else
    {
        cout << "NO" << endl;
    }

    return 0;
}
```

<hr>

# Java
```java
import java.util.Scanner;

public class EvenSplit {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int w = scanner.nextInt();

        if (w > 2 && w % 2 == 0) {
            System.out.println("YES");
        } else {
            System.out.println("NO");
        }

        scanner.close();
    }
}
```
