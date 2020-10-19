# constexpr-if

Create an add function with the help of `if constexpr` that accepts all those cases: 

```cpp
std::string test{"hello"};
auto val1 = add(1,1);
auto val2 = add(1.1,3);
auto val3 = add(test,1.0);
auto val4 = add("hello",1.0);
```
     