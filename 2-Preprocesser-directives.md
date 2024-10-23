# Preprocesser Directives 
Imagine that you want to eat blueberries, but sadly, blueberries don't grow in your region. Instead of just wishing, you can import them from other regions and eat them happily.
There's a fair reason for giving the above example.
Preprocesser Directives are instructions given to compiler's preprocesser. You probably didn't understood the sentence you just read, but I'll explain that right now.
Focus on the blueberries example. If you want to eat them, but they don't grow in your region, you have to import them. Similarly, compiler's preprocesser can do certain tasks, that may be required for your program to fucntion properly.
And preprocesser directives are just the instructions you give to it.
## Writing Code
Now that you have understood concept of preprocesser directives, we can focus on using them in our code.
All the preprocesser directives begin with '#'. This is the convention used for them in C++.
There are quite a few preprocesser directives, but for this lesson, we'll focus on 3 of them only.
#### `#include`
Like you were importing and using (eating) blueberries from a different region, `#include` allows you to use contents of a file. Well, not any file, it could be a `.cpp`(C++ file),`.hpp`,`.c`(C file) or `h`. You're probably familiar with `.cpp` and `.c` but you may or may not `.h` or `.hpp`. Well, Those are header files. They're discussed in later lessons.
```cpp
#include <iostream>
```
This includes a header iostream. You'll get to know a little bit about it in the next lesson.
#### `define`
Macros are pieces of code that are expanded by preprocesser by their definition.
The simplest work of a macro is, whenever the compiler sees a macro in your code, it replaces that macro with its defined value.
Here's how you would define a macro in a line of code:
```cpp
#define myMacro 0
```
This is an Object-like macro.
There are quite a few types of macros, but in practical terms, most commonly used ones are Object-like and Function-like macros, Out of which we'll focus on Object-like only because we haven't got to Fucntions chapter yet.
Look at this code :
```cpp
int main(){
    return 0;
}
```
Now we'll add two lines:
```cpp
#define myFunction int main()
#define myReturn return 0;
```
We can rewrite that code like this:
```cpp
#define myFunction int main()
#define myReturn return 0;

myFunction {
    
    myReturn
}
```
Quite Cool, Right? myFucntion gets replaced with `int main()` and `myReturn` gets replaced with `return 0;`, resulting in proper execution of code.