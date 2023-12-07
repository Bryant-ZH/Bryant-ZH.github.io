# `Bryant-ZH's Portfolio`

This is my home page! My name is Bryant and I am a student at [Cal State Fullerton](http://www.fullerton.edu/) and my major is computer science.

[My github profile](https://github.com/Bryant-ZH)

### Some labs I have done in the past:

CPSC 120
--- 
**Lab 3, Part 2**
```Cpp
int DateDifference(int start_month, int start_day, int start_year,
                   int end_month, int end_day, int end_year) {
  int start_date = JulianDay(start_month, start_day, start_year);
  int end_date = JulianDay(end_month, end_day, end_year);
  int difference = (end_date - start_date);
  return difference;
}
```
>I really enjoyed this part of the lab because it was quite lengthy at the time and seeing it work was awesome.  
>This lab also helped us understand how to write functions and call them.  It was also cool to be able to turn 
>two dates into a Julian date and give the difference between them. 

**Lab 4, Part 1**
```Cpp
int main(int argc, char const *argv[]) {
  double mil{0.0};
  std::cout << "Enter ml: ";
  std::cin >> mil;

  double tsp = MlToTsp(mil);
  double tbsp = MlToTbsp(tsp);
  double ounce = MlToOz(tbsp);
  double cups = MlToCup(ounce);

  std::cout << mil << " ml = ";
  std::cout << tsp << " tsp = ";
  std::cout << tbsp << " tbsp = ";
  std::cout << ounce << " oz = ";
  std::cout << cups << " cups\n";
  return 0;
}
```
>I liked this lab because it was somewhat challenging at the time.  
>I also believe this is the first time we started to implement header files into our labs as well as calling 
>functions.  The program itself is also helpful since it converts milliliters into other measurements. 

**Lab 5, Part 2**
```Cpp
int TruncateDouble(double decimal_number) {
  double integer_part = (trunc(decimal_number));
  int converted_integer_part = 0;

  if (integer_part >= std::numeric_limits<int>::max()) {
    converted_integer_part = std::numeric_limits<int>::max();
  } else if (integer_part <= std::numeric_limits<int>::min()) {
    converted_integer_part = std::numeric_limits<int>::min();
  } else {
    converted_integer_part = static_cast<int>(trunc(integer_part));
  }

  return converted_integer_part;
}
```
>This lab was interesting to me because we got to use the trunc() function and static_cast to convert doubles
>into integers.  We also had to check to see if we could convert by using std::numeric_limits<int>::max() and
>std::numeric_limits<int>::min().  This was needed in order to convert a given decimal number into a number 
>with a fraction.

