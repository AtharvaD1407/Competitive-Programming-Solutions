# Python
```python
n = int(input())

for i in range(n):
    w = input()

    if len(w) > 10:
        print(f"{w[0]}{len(w)-2}{w[-1]}")
    else:
        print(w)
```

<hr>

# C++
```c++
#include <iostream>
#include <string>
using namespace std;

int main()
{

    int n;
    string w;

    cin >> n;

    for (int i = 0; i < n; i++)
    {
        cin >> w;

        if (w.length() > 10)
        {
            cout << w[0] << w.length() - 2 << w[w.length() - 1] << endl;
        }
        else
        {
            cout << w << endl;
        }
    }

    return 0;
}
```

<hr>

# Java
```java
import java.util.Scanner;

public class TooLongWords {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int n = scanner.nextInt();
        scanner.nextLine(); 

        for (int i = 0; i < n; i++) {
            String w = scanner.nextLine();

            if (w.length() > 10) {
                System.out.println(w.charAt(0) + "" + (w.length() - 2) + w.charAt(w.length() - 1));
            } else {
                System.out.println(w);
            }
        }

        scanner.close();
    }
}
```