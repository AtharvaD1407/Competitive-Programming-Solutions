# Python
```python
username = input()

distinct_characters = set(username)

count_distinct = len(distinct_characters)

if count_distinct % 2 == 0:
    print("CHAT WITH HER!")
else:
    print("IGNORE HIM!")
```

<hr>

# C++
```c++
#include <iostream>
#include <set>
#include <string>
using namespace std;

int main()
{
    string username;
    cin >> username;

    set<char> distinct_characters(username.begin(), username.end());

    int count_distinct = distinct_characters.size();

    if (count_distinct % 2 == 0)
    {
        cout << "CHAT WITH HER!" << endl;
    }
    else
    {
        cout << "IGNORE HIM!" << endl;
    }

    return 0;
}
```

<hr>

# Java
```java
import java.util.Scanner;
import java.util.HashSet;

public class ChatDecision {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String username = scanner.nextLine();

        HashSet<Character> distinctCharacters = new HashSet<>();
        for (char c : username.toCharArray()) {
            distinctCharacters.add(c);
        }

        int countDistinct = distinctCharacters.size();

        if (countDistinct % 2 == 0) {
            System.out.println("CHAT WITH HER!");
        } else {
            System.out.println("IGNORE HIM!");
        }

        scanner.close();
    }
}
```
