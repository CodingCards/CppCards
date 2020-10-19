## Solution

```cpp
int calcSquare(int number){
    return (number * number)
}

int f(int i)
{
    int res = 0;
    switch(i)
    {
        case 1:
            res = calcSquare(i);
            [[fallthrough]];
        [[likely]] case 2:
            res = calcSquare(i);
            break;
        [[unlikely]] case 3:
            res = calcSquare(i);
            break;
    }
    return res;
}

int main() {
    f(1);
    f(2);
    f(3);
    return 0;
}
```

## Note
```[fallthrough]``` was actually implemented in C++17, just added it here for completion.

## Links

- [Cpp Reference: attribute specifier sequence](https://en.cppreference.com/w/cpp/language/attributes)
