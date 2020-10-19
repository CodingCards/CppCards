## Solution part 1
```cpp
#include<iostream>
#include<unordered_map>
#include<string>

int main() {
    std::unordered_map<int,std::string> portServiceMap = {{21,"FTP"},{80,"http"},{22,"ssh"}};
    for(auto const&[port, service] : portServiceMap) {
        std::cout << "Port: " << port << "Service:" << service; 
    }    
    return 0;
}
```

## Solution part 2
```
#include<utility>
#include<tuple>
#include<string>

int main() {

    std::pair<int, std::string> pair = {21,"Ftp"};
    const auto tuple = std::make_tuple(21, "Ftp", "TCP");

    auto const& [port, service] = pair;
    auto const& [port2,service2,protocol] = tuple;
    
    return 0;
}
```

## Links

- [Cpp Reference](https://en.cppreference.com/w/cpp/language/structured_binding)
