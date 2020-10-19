## Solution

```cpp
#include <iostream>
#include <date/date.h>

int getAgeInYears(date::year_month_day dayOfBirth) {
    // timestamp
    auto now = std::chrono::system_clock::now();
    // convert to sys_days
    date::sys_days nowSysDays = date::floor<date::days>(now);
    // convert to year_month_day (same as dayOfBirth)
    date::year_month_day nowYmd = date::year_month_day{nowSysDays};
    auto ageInDays = date::local_days{nowYmd} - date::local_days{dayOfBirth};
    date::years ageInYears = std::chrono::duration_cast<date::years>(ageInDays);
    return ageInYears.count();
}

int main()
{
    using namespace date;
    constexpr auto x1 = 1981_y/March/11;
    constexpr auto x2 = October/07/1991;
    constexpr auto x3 = 26_d/October/2015;
    std::cout << "You are " << getAgeInYears(x1) << " years old\n";
    std::cout << "You are " << getAgeInYears(x2) << " years old\n";
    std::cout << "You are " << getAgeInYears(x3) << " years old\n";
    return 0;
}
```

## Links

[https://en.cppreference.com/w/cpp/chrono](cppreference)
[https://github.com/HowardHinnant/date](https://github.com/HowardHinnant/date)
