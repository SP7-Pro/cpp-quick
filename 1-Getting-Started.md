# Getting Started
## Introduction 
Getting started can be the most challenging point of learning a very new concept, after some time, you'll progress further and the concepts will be a piece of cake.
## Installing an IDE
**IDE stand for integrated development environment.** It is what developers use to edit and debug their code. Code Editors can be used too, But they aren't as feature-rich as an IDE. Also if your program ran into a critical error, IDEs can assist you greatly in debugging, making the devlopement process way faster.
The first step is to choose the IDE that you want to use. Some of the well-known ones are Microsoft Visual Studio, Code::Blocks, Eclipse Kepler, Orwell C/C++ Dev and Codelite.
This series does not teach you to install and configure them. Instead, you'ld follow the instructions provided on webpages of the IDE you're using. I'll link the downloads to the IDEs :
- [Microsoft Visual Studio](https://visualstudio.microsoft.com/downloads/) 
- [Code::Blocks](https://www.codeblocks.org/downloads/)
- [Eclipse Kepler](https://www.eclipse.org/downloads/packages/release/kepler/sr2/eclipse-ide-cc-developers)
IDEs will install an compiler for you. No need to worry about compiler installation!
## Writing Code
Let's get to writing some actual code.
```cpp
// main gets called when programs begins executing 
int main(){
    every piece of code you write here gets executed 
    return 0; // returns 0 ( success ) 
}
```
What you see above, is the minimum code required to make a program that when compiled, compiles successfully and when ran, just executes and finishes.
## Functions 
From the code snippet you saw above, `main` is the fucntion that gets called when your program starts executing. Functions are a complex topic, they're explained later on in this series, but for now I'll give a simple explanation. You can think of functions as a vending machine, you give some coins in it and get your desired drink. Fucntions can actually take some values or nothing, like the coin to the vending machine, that are discussed about later on in this series. when `main` is called, all the code in it gets executed. And you see that `return 0;`? That's a return code! After program finishes executing, it hands a value to the operating system. This value is like a secret code, that can indicate how program has finished executing. On most systems, the return code for success is 0 and failure is 1.
## Return Codes on system
Other than 0 and 1, operating systems have a vast collection of return codes. I will mention some return codes on Unix and Windows and their meaning :
**Unix Return Codes**
| Return Codes | Meaning |
|:------------:|:--------|
|0             |Success  |    
|1             |General Error  |
|127           |Command not found |
|128           |Invalid argument to exit |

You can read more about return codes of Unix [here](https://www.gnu.org/software/bash/manual/bash.html#Exit-Status).
**Windows Return Codes**
| Return Codes | Meaning |
|:------------:|:--------|
|0             |Success  |
|1             |Invalid Function |
|5             |Access Denied |
|8             |Out of Memory |

Windows has alot that just these that are mentioned here, It has 500 distinct return codes! You can read about them [here](https://learn.microsoft.com/en-us/windows/win32/debug/system-error-codes--0-499-).