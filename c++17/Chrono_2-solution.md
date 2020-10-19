## Solution

```cpp
#include <chrono>
#include <thread>

int test() {
  std::this_thread::sleep_for(std::chrono::seconds(2));
    return 0;
}

using chrono_frames = std::chrono::duration<unsigned int,std::ratio<1,60>>;

int main() {
   auto t1 = std::chrono::system_clock::now();
   test();
   auto t2 = std::chrono::system_clock::now();
   auto myFrames = std::chrono::duration_cast<chrono_frames>(t2-t1).count();

   return 0;
}
```

## Links

- [Cpp Reference](https://en.cppreference.com/w/cpp/header/chrono)
- [(youtube) Meeting C++ 2019 Opening Keynote - Howard Hinnant](https://www.youtube.com/watch?v=adSAN282YIwo)
