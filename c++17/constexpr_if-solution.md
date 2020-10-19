## Solution

```cpp
template<typename T, typename M>
auto add(T t1, M t2) {
    if constexpr(std::is_same_v<T,const char*> ||
                 std::is_same_v<T,std::string>) {
        return t1 + std::to_string(t2);
    } else {
        return t1+t2;    
    }
}
```

## Links

- [Simplify Code With 'if constexpr' in C++17](https://dzone.com/articles/simplify-code-with-if-constexpr-in-c17-1)
- [Cpp Reference](https://en.cppreference.com/w/cpp/language/if)
