## Solution

```cpp
#include <span>
#include <vector>

int add(std::span<int> vals) {
    int sum=0;
    for(auto const& val : vals) {
        sum += val;
    }
    return sum;
}


int main() {
    int ca[]{2,3,4,5};
    std::vector v{1,2,3,4,5};
    std::array a{1,2,3,4,5};
    int *p = ca;
    
    add(ca);
    add(v);
    add(a);
    
    add({p,4});
    // or
    add(std::span{p,4});

    return 0;
}
```

## Links

- [Cpp Reference](https://en.cppreference.com/w/cpp/container/span)
