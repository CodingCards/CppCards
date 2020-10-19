## Solution

```cpp
#include<iostream>
#include<experimental/source_location>

void log(std::string_view message,
         const std::experimental::source_location& location = std::experimental::source_location::current())
{
    std::cout << "info:"
              << location.file_name() << ":"
              << location.line() << ' '
              << message << '\n';
}

int main()
{
    log("Hello world!");
}
```

## Links

- [Cpp Reference](https://en.cppreference.com/w/cpp/utility/source_location)
