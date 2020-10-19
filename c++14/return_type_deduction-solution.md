# Keyword auto return value

```
template <typename T1, typename T2>
auto add(T1 t1, T2 t2) {
   return t1+t2;
}

int main() {
    return add(4,3);
}
```

## Links
- [Cpp Reference](https://en.cppreference.com/w/cpp/language/auto)

### Note
Since C++20, the trailing return "trick" with ```decltype``` is not necessary anymore.
(Abbreviated function template)
- [Cpp Reference](https://en.cppreference.com/w/cpp/language/function_template#Abbreviated_function_template)


