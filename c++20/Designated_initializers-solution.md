## Solution

```cpp
struct AwesomeStruct {
    int anInt;
    int anotherInt;
    float aFloat;
};

int main() {
    AwesomeStruct{.anInt = 1, .anotherInt = 2, .aFloat = 3.2f};
    return 0;
}
```

## Links

- [Cpp Reference](https://en.cppreference.com/w/cpp/language/aggregate_initialization#Designated_initializers)
