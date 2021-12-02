# Reference wrapper

```
#include <iostream>
#include <vector>
#include <numeric>
#include <functional>

int main() {
    std::vector<int> l(10);
 
    std::iota(l.begin(), l.end(), 0);
    std::vector<std::reference_wrapper<int>> v(l.begin(), l.end());

    for (const auto& i : v){
       std::cout << i.get() << ' ';
    }
}
```

## Links
- [Cpp Reference](https://en.cppreference.com/w/cpp/utility/functional/reference_wrapper)