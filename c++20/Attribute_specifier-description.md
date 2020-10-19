# Attribute specifier 

Use Attributes (`likely, unlikly and fallthrough`) to optimize the given code and make them compile.

 - `case 1:` has no preference
 - `case 2:` is the most likely branch
 - `case 3:` is tht most unlikely branch

```cpp
int calcSquare(int number){
    return (number * number);
}

int f(int i)
{
    int res = 0;
    switch(i)
    {
        case 1: 
            res = calcSquare(i);
        case 2:
            res = calcSquare(i);
            break;
        case 3:
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


