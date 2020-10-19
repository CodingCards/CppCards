## Solution

```cpp
#include <compare>
struct AnInt {
  int value;
  constexpr AnInt(int value): value{value} { }
  std::strong_ordering operator<=>(const AnInt&) const = default;
};

int main() {
    AnInt test1(3);
    AnInt test2(4);    
    
    if (test1 < test1) {
        return 1;
    }
    return 0;
}
```

## Links

- [Cpp Reference - Three way comparison](https://en.cppreference.com/w/cpp/language/operator_comparison#Three-way_comparison)
- [Cpp Reference - compare header](https://en.cppreference.com/w/cpp/header/compare)
