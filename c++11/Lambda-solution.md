## Solution part 1

```cpp
auto lambda = []{};
```

## Solution part 2

```cpp
int main (){
    auto sum = [](auto x, auto y) { return x + y; };
    sum(2,3);
}
```

## Links

- [Cpp Reference](https://de.cppreference.com/w/cpp/language/lambda)


## general knowledge
structure of a lambda
```cpp
[captures] (params) {body}
```

captures:
 - `[]` captures nothing
 - `[&]` captures all variables used in the lambda by reference
 - `[=]` captures all variables used in the lambda by value
 - `[this]` captures `this` pointer by value
