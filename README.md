# Kofu is usually developed on the UGDS open source platform, which is a student-led open source platform. It is recommended that you develop Kofu on the UGDS open source platform.
<a href="https://git.jtopgame.top/zhiyu/Kofu">UGDS</a>

![Kofulogo](./readmeimg/kofu.png)
# Kofu
Make programming no longer out of reach

## TODO😍
- [x] Basic syntax
- [ ] Loop
- [ ] IDLE with syntax highlighting
- [ ] VSCode plugin
- [ ] Allow files to use command commands

## How to participate in the development of Kofu? 👍
This project requires Python 3.10
Warning: Due to the limitation of PyO3 library, only Python 3.10 is supported. Thank you for your cooperation (ps: If you insist on using Python 3.10 or above, please see "How to compile Rust library?" below)
Use pip to install the Kofu_Rust_Lib.whl file in the root directory of the project. This is a Python 3.10 version of the Rust library used to call Rust code
```bash
pip install ./kofu_rust_lib-0.1.2-cp310-none-win_amd64.whl
```
After cloning the project to your local, open the kofu_include.py in the project. This is the interpreter of Kofu
You can modify this file and compile it into a pyd file after modifying it. At this time, all the Python programs in IDLE, interactive mode, etc. that call kofu and have not been modified under this project are the new syntax you modified
If you want to develop a Rust library, please install Rust and Rust-Analyzer plugins for VSCode, wait for the scan to complete, edit lib.rs, and then compile it into a whl file and install it according to the method in "How to compile Rust library?". After testing, modify the command line instructions in README.md.

## How to compile Rust library? 🧐
First, you need to install the Rust environment, pip library, Rust-Analyzer for VSCode, and Rust plugin.
```bash
pip install maturin
```
Then set your Python script directory as an environment variable, and then execute
```bash
maturin build
```
Then the Kofu-x.x.x-cp(your Python version number)-none-system_architecture.whl file will be generated in the target/wheels directory. Install it into your Python environment.
Warning: If you modify the lib.rs file, please be sure to compile a wheel file for Python 3.10, otherwise you will violate the Kofu Developer Agreement.

## Can Kofu be called a programming language? 🤓
### Look at what AI says
#### Kimi
Of course. The definition of a programming language does not strictly restrict its implementation. Even an interpreter or compiler implemented in another programming language can be considered an independent programming language as long as it has its own grammatical rules, semantics, and the ability to perform specific tasks.

The core of a programming language lies in its design and functionality, not its underlying implementation. For example, Python itself is implemented in C, but this does not prevent Python from becoming a widely used programming language. Similarly, if your "programming language" provides unique syntax and functionality and can be used to write programs, then it can be called a programming language.

In addition, programming languages ​​can be designed for a variety of purposes, such as education, application in a specific field, or simply to explore the possibilities of programming language design. As long as your language can meet these purposes and there is a user group willing to use it, it is a valid programming language.

#### Wen Xin Yi Yan (3.5)
To determine whether a system can be called a "programming language", we need to evaluate it based on the basic definition and characteristics of programming languages. A programming language is an artificial language used to define, develop, and maintain computer programs, usually including syntax, semantics, and a set of standard libraries or APIs.

From your problem description, we can extract the following key information:

The interpreter is written in Python: This describes the technical details of implementing the interpreter of the language, but does not affect the nature of the language itself. The interpreters or compilers of many modern programming languages ​​are also implemented in other programming languages ​​(such as C, C++, Java, etc.).
It has a lot of unique syntax: This is an important feature of a programming language. Each programming language has its own unique syntax rules that define how to write valid programs.

Based on this information, we can make the following inferences:

Syntax uniqueness: Since the language has a unique syntax, it meets a basic feature of a programming language. Syntax is the basis of a programming language, which defines how programs are written and structured.
Interpreter exists: Although the interpreter is written in Python, it is still a valid interpreter that can understand and execute programs written in the language. The existence of the interpreter makes the language executable, which is an important property of a programming language.
Conforms to the definition: According to the above characteristics, the language meets the definition of a programming language. It has its own grammatical rules and an interpreter that can execute these rules, so it can be considered a programming language.

In summary, even if the interpreter of your "programming language" is written in Python and it has a lot of unique syntax, it can still be called a programming language. This is because its syntax and interpreter together constitute the two core elements of a programming language.

#### ChatGPT (4o mini)
Yes, even if your "programming language" is implemented in Python, as long as it has its own syntax, semantics and rules, it can be called a programming language. The definition of a programming language does not depend on its implementation language. The key lies in whether it provides ways and tools to express calculations.

If your language has unique syntax and functions that can be used to write programs and solve problems, then it is a programming language. The interpreters or compilers of many languages ​​are implemented in other languages, such as Python implemented in C, Scala implemented in Java, etc. What matters is whether you can use this language for effective programming.

## Some Q&A🎺
Q: When will the compiler be developed? A: This... I really don't know how to write it!
Wait until Q...

## List of programming languages ​​used (unchecked ones may be used in the future, checked ones are in the current project)😍
- [x]Python
- [ ]Html (including html javascript css)
- [x]Rust

## Current bug list💀
1. Variables cannot be called
2. Command code cannot be used in files

## Python IDE recommendation❤️
- PyCharm
- VSCode
- Sublime Text

## Currently found unfixable bugs💀
1. Command cannot be used in Turtle Editor

## Kofu Developer Agreement😍
- Python 3.10 version is preferred❤️
- Kofu uses MIT protocol❤️
- Kofu developers are not allowed to leak user privacy by any means such as Trojan virus❤️
- Kofu is prohibited from being used for any illegal or criminal activities❤️

## What will happen if the Kofu Developer Agreement is violated? 🤓
- Lifelong ban from Kofu development💀
- Banned by zhiyu's other projects💀
- Prohibited from working as an outsourcer on UGDS project💀

## Future development plans🤔
- Flask-based web backend

## Some thoughts💭
### Zhiyu
Zhiyu is the founder of Kofu language. He is a student who loves programming. One of his ideas is to give birth to Kofu language.
#### First😘
I am Zhiyu, and also the founder of Kofu language. When I created this language, I just wanted to make programming no longer out of reach. Programming should be close to the people, so that everyone can have their own App. That's how Kofu came about. I hope everyone can like this language, and I hope Kofu can help everyone.
#### Behind the scenes-a wonderful idea💭
I have always liked programming, and I have come into contact with many programming languages, such as C++ Java, but they are too cumbersome. One day, it was an ordinary Saturday. I was sitting in the car and suddenly thought of a question. Why are programming languages ​​so complicated? Isn't there a simple and easy-to-learn programming language? So I went home and thought about it. Suddenly, an idea came to me. That is, to make a programming language myself. Kofu was born.
#### Behind the scenes-school🏫
I have to go to school again today. I thought of Kofu again, but I was at school. The school's Windows all-in-one machine did not have a Python environment, so I couldn't write Kofu at all. I suddenly thought, hey! Isn't my club a programming club? After getting the teacher's approval, I started to build a Python environment, install Git, clone the project, log in to the Git account, and start writing Kofu.
#### Behind the scenes - License📃
Not long before I wrote this text, I decided to let Kofu use the MIT license. MIT is a very permissive license. As long as you sign my name on your project, you can use my code at will. Although my code will be taken away, I still welcome you to use my project
#### Finally🤓
I hope Kofu can help everyone, make programming no longer out of reach, and make programming easy to learn.
I also hope that Kofu developers can abide by the Kofu Developer Agreement, protect user privacy, and not participate in illegal activities.
Finally, thank you for your support!
### undefined
undefined is one of the developers of the Kofu language, and his remarks are to be added

Happy coding!
