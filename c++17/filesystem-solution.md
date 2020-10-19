## Solution

```cpp
#include <filesystem>
#include <vector>


std::vector<std::string> listFiles(std::string const& path) {
    std::string path_name = ".";

    std::vector<std::string> names;

    for (auto &entry : std::filesystem::directory_iterator(path_name)) {
        names.push_back(entry.path().filename());
    }
    return names;
}

int main() {
    auto files = listFiles(".");
    return 0;
}
```

## Links

- [Cpp Reference](https://en.cppreference.com/w/cpp/header/filesystem)
