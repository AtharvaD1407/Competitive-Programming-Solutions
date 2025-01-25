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
