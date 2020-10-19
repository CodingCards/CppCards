## Solution

```cpp
#include <vector>
#include <ranges>
#include <iostream>
 
int main()
{
    std::vector<int> ints{0,1,2,3,4,5};
    auto even = [](int i){ return 0 == i % 2; };
    auto square = [](int i) { return i * i; };
 
    for (int i : ints | std::views::filter(even) | std::views::transform(square)) {
        std::cout << i << ' ';
    }
}
```

## Links

- [Cpp Reference](https://en.cppreference.com/w/cpp/ranges)
- [https://ericniebler.github.io/range-v3/](https://ericniebler.github.io/range-v3/)
