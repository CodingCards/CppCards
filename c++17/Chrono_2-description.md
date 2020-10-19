# Chrono-2

With the help of chrono, count how many frames the execution of function test took, given a framerate of 60FPS.

```cpp
int test() {
    std::this_thread::sleep_for(std::chrono::seconds(2));
    return 0;
}
   
int main() {
   test();

   return 0;
}
```