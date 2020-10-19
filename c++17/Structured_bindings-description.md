# Structured bindings

### Part 1
Create expressive names within a range base for loop
with the help of structured bindings 

```cpp
std::map<int,std::string> portServiceMap = {{21,"FTP"},{80,"http"},{22,ssh}}
for(? : portServiceMap) {
    ?
    std::cout << "Port: " << ? << "Service:" << ?; 
}
```

### Part 2     
Create expressive names for the following variables

```cpp
std::pair<int, std::string> portMap = {21,"Ftp"};
const auto tuple = std::make_tuple(21, "Ftp", "TCP");
```