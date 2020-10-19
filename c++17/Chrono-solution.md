## Solution

```cpp
#include <chrono>

int test() {
   return 0; 
}


int main() {
    auto t1 = std::chrono::system_clock::now();
    test();
    auto t2 = std::chrono::system_clock::now();
    auto nanoseconds = std::chrono::duration_cast<std::chrono::nanoseconds>(t2-t1).count();
    
}
```

## Links

- [Cpp Reference](https://en.cppreference.com/w/cpp/header/chrono)
- [(youtube) Meeting C++ 2019 Opening Keynote - Howard Hinnant](https://www.youtube.com/watch?v=adSAN282YIwo)
