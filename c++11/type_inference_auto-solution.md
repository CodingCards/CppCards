
### C++98

Before C++ 11 we had to use iterators which in some examples could be really
long and incomprehensible
```cpp
    std::vector<int> data(10);
    for (std::vector<int>::iterator it = data.begin() ; it != data.end(); ++it) {
        std::cout << ' ' << *it;
    }
```

### C++11
Now with the new keyword ```auto``` we can do:

```cpp
   std::vector<int> data(10);
   for(auto it = data.begin(); it != data.end(); it ++) {
      std::cout << ' ' << *it;
   }
```

Or even simpler:

```cpp
   std::vector<int> data(10);
   for(auto const& val : data) {
       std::cout << ' ' << val;
   }
```

### All together
```
#include <vector>
#include <iostream>

int main() {
    std::vector<int> data(10);

    for (std::vector<int>::iterator it = data.begin() ; it != data.end(); ++it) {
        std::cout << ' ' << *it;
    }
    for(auto it = data.begin(); it != data.end(); it ++) {
        std::cout << ' ' << *it;
    }
       
    for(auto const& val : data) {
        std::cout << ' ' << val;
    }
    return 0;
}

```

## Links
- [Cpp Reference](https://en.cppreference.com/w/cpp/language/auto)
