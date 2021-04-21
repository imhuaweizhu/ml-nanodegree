# Machine Learning Engineer Nanodegree Program - Udacity

## Software eingieering practices

Production code: software running on production servers to handle live users and data of the intended audience. 

Production quality code: code that meets expectations in reliability, efficiency, etc., for production.

### Always write clean and modular code

#### Two General Rules

1. Clean: readable, simple and consise (for collaboration and maintainability).
2. Modular: logically broken up into functions and modules (for reusablity and efficiency).

#### Refactoring your code by following the above rules

It isn't easy to write your best code while you're still trying to just get it working. So we need to go back, clean and modularize your program after you've got the coding task working. Restructure your code to improve its internal structure, without changing its external functionality.

##### Rule #1. Refactoring your code: cleanize code

Reference the style guideline for your choice of language. 

C++: Code style and coding guidelines https://named-data.net/doc/ndn-cpp-dev/0.4.0/code-style.html

Python: PEP 8 -- Style Guide for Python Code https://www.python.org/dev/peps/pep-0008/?#code-lay-out

###### (1). Use meaningful names

------ Be descriptive and imply type. Long names != descriptive names. For example: verbs for functions and nouns for variables, is_ or has_ for booleans

------ Be consistent but clearly differentiate. For example: age_list and age is easier to differentiate than ages and age.

------ Avoid abbreviations unless the phrase will be used a lot in the program

###### (2). Use whitespace properly
------ Organize your code with consistent indentation. For example: the standard is to use 4 spaces for each indent.

------ Separate sections with blank lines to keep your code well organized and readable.

------ Try to limit your lines to around 79 words/characters including comments.

------ Refer the style guideline for your language. For example: http://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines#S-philosophy

##### Rule #2. Refactoring your code: modularize code

------ (1) Don't Repeat Yourself

Generalize and consolidate repeated code in functions or loops.

------ (2) Abstract out logic to improve readability

Abstracting out code into a function not only makes it less repetitive, but also improves readability with descriptive function names. But do not over-engineer this.

------ (3) Minimize the number of entities (functions, classes, modules, etc.)

There are tradeoffs to having function calls instead of inline logic. Creating more modules doesn't necessarily result in effective modularization.

------ (4) Functions should do one thing

Generally, if there's an "and" in your function name, consider refactoring. Each function you write should be focused on doing one thing.

------ (5) Try to use fewer than three arguments per function

Try to use no more than three arguments when possible. his is not a hard rule and there are times it is more appropriate to use many parameters. If your function has a lot of parameters, you may want to rethink how you are splitting this up.

##### Rule #3. Refactoring your code: make your efficient code

------ (1) Reduce time complexity
------ (2) Reduce space complexity (memory/storage usage)

### Documentation

#### Types of documentation
1. In-line comments
2. Function-level and Module-level comments (using Docstrings)
3. Project-level comments (using Docstrings): Your project should absolutely come with a README file. At a minimum, it should explain what it does, list its dependencies, and provide sufficiently detailed instructions on how to use it.







