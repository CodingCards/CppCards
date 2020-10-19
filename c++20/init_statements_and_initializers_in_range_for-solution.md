## Solution

```cpp
int main() {
    std::vector<std::string> names = {"lisa","sven","karl","hugo"};
    for (int i = 0; auto name : names) // the init-statement (C++20)
        std::cout << i++ << ':' << name<<"\n";
}
```

## Links

- [Cpp Reference](https://en.cppreference.com/w/cpp/language/range-for)
