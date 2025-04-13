
### 1.  `max(a, b)` and `min(a, b)`

**Questions:**
1. How do you find the larger of two integers?
2. How do you compare and pick the smaller of two values?

- **Example:**
```cpp
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
    int a = 15, b = 30;
    cout << max(a, b) << "\n"; // 30
    cout << min(a, b) << "\n"; // 15
}
```

---

<!--
###  `sort(begin, end)`

**Questions:**
1. How do you sort a list of numbers in ascending order?
2. How can you sort a string alphabetically?

✅ **Example:**
```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;

int main() {
    vector<int> nums = {4, 2, 7, 1};
    sort(nums.begin(), nums.end());
    for (int n : nums) cout << n << " "; // 1 2 4 7
}
```

---

###  `reverse(begin, end)`

**Questions:**
1. How do you reverse a vector of numbers?
2. How do you reverse the characters of a string?

✅ **Example:**
```cpp
#include <iostream>
#include <algorithm>
#include <string>
using namespace std;

int main() {
    string word = "hello";
    reverse(word.begin(), word.end());
    cout << word; // olleh
}
```

---

###  `accumulate(begin, end, initial)`

**Questions:**
1. How do you get the total of all elements in a list?
2. How can you sum all integers from a file or input?

✅ **Example:**
```cpp
#include <iostream>
#include <vector>
#include <numeric>
using namespace std;

int main() {
    vector<int> data = {1, 2, 3, 4};
    int total = accumulate(data.begin(), data.end(), 0);
    cout << total; // 10
}
```

---

###  `count(begin, end, value)`

**Questions:**
1. How many times does a specific number appear in a list?
2. How do you count characters like `'a'` in a string?

✅ **Example:**
```cpp
#include <iostream>
#include <algorithm>
#include <vector>
using namespace std;

int main() {
    vector<int> nums = {1, 3, 3, 3, 5};
    cout << count(nums.begin(), nums.end(), 3); // 3
}
```

---

###  `find(begin, end, value)`

**Questions:**
1. How do you search for a number in a list?
2. How can you check if a character exists in a string?

✅ **Example:**
```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;

int main() {
    vector<int> nums = {10, 20, 30};
    if (find(nums.begin(), nums.end(), 20) != nums.end())
        cout << "Found!";
    else
        cout << "Not Found!";
}
```

---
-->

### 2. `to_string()`

**Questions:**
1. How do you convert an integer to a string?
2. How can you create messages like "Score: 99"?

- **Example:**
```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    int score = 99;
    string result = "Score: " + to_string(score);
    cout << result;
}
```

---

### 3. `stoi()`, `stof()`, etc.

**Questions:**
1. How can you convert a string `"100"` to an integer?
2. How do you process numeric strings from user input?

- **Example:**
```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string s = "123";
    int num = stoi(s);
    cout << num + 1; // 124
}
```

---

### 4. `getline(cin, str)`

**Questions:**
1. How do you read full-line input (including spaces)?
2. How do you take a full sentence as input?

✅ **Example:**
```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string line;
    getline(cin, line);
    cout << "You entered: " << line;
}
```

---

### 5. `swap(a, b)`

**Questions:**
1. How do you exchange values of two variables?
2. How do you swap elements in a sorting algorithm?

✅ **Example:**
```cpp
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
    int x = 3, y = 7;
    swap(x, y);
    cout << x << " " << y; // 7 3
}
```

---

