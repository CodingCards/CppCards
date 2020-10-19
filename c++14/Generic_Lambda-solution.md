# Generic Lambda

```
#include <iostream>
#include <string>

int main() {
   auto add = [](auto x, auto y){return x+y;};
   std::string str =  add(std::string("3"),std::string("2.3"));
   float f = add(3,2.3);
   return 0;
}
```

##Links
-  [isocpp](https://isocpp.org/wiki/faq/cpp14-language#generic-lambdas)