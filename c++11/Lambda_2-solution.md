## Solution

```cpp
int main()
{
  int a = 5;
    
  class __lambda_4_16
  {
    public: 
    inline /*constexpr */ int operator()(int b) const
    {
      return a + b;
    }
    
    private: 
    int & a;
    
    public:
    __lambda_4_16(int & _a)
    : a{_a}
    {}
    
  };
  
  __lambda_4_16 sum = __lambda_4_16{a};
}
```

## Links

- [Cpp Reference](https://de.cppreference.com/w/cpp/language/lambda)
- [cppinsights](https://cppinsights.io/)