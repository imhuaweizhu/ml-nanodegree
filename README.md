# Machine Learning Engineer Nanodegree Program - Udacity

## Software eingieering practices

Production code: software running on production servers to handle live users and data of the intended audience. 

Production quality code: code that meets expectations in reliability, efficiency, etc., for production.

### 1. Always write clean, modular, and efficient code

It isn't easy to write your best code while you're still trying to just get it working. So we need to go back, clean and modularize your program after you've got the coding task working. Restructure your code to improve its internal structure, without changing its external functionality. 

(1). Clean: readable, simple and consise (for collaboration and maintainability).

(2). Modular: logically broken up into functions and modules (for reusablity and efficiency).

(3). Efficient: improve performance of production code

#### Rule #1. Refactoring your code: cleanize code

Reference the style guideline for your choice of language. 

(1). C++: Code style and coding guidelines (https://named-data.net/doc/ndn-cpp-dev/0.4.0/code-style.html)

(2). Python: PEP 8 -- Style Guide for Python Code (https://www.python.org/dev/peps/pep-0008/?#code-lay-out)

##### (1) Use meaningful names

-- Be descriptive and imply type. Long names != descriptive names. For example: verbs for functions and nouns for variables, is_ or has_ for booleans

-- Be consistent but clearly differentiate. For example: age_list and age is easier to differentiate than ages and age.

-- Avoid abbreviations unless the phrase will be used a lot in the program

##### (2) Use whitespace properly
-- Organize your code with consistent indentation. For example: the standard is to use 4 spaces for each indent.

-- Separate sections with blank lines to keep your code well organized and readable.

-- Try to limit your lines to around 79 words/characters including comments.

-- Refer the style guideline for your language. For example: http://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines#S-philosophy

#### Rule #2. Refactoring your code: modularize code

##### (1) Don't Repeat Yourself

Generalize and consolidate repeated code in functions or loops.

##### (2) Abstract out logic to improve readability

Abstracting out code into a function not only makes it less repetitive, but also improves readability with descriptive function names. But do not over-engineer this.

##### (3) Minimize the number of entities (functions, classes, modules, etc.)

There are tradeoffs to having function calls instead of inline logic. Creating more modules doesn't necessarily result in effective modularization.

##### (4) Functions should do one thing

Generally, if there's an "and" in your function name, consider refactoring. Each function you write should be focused on doing one thing.

##### (5) Try to use fewer than three arguments per function

Try to use no more than three arguments when possible. his is not a hard rule and there are times it is more appropriate to use many parameters. If your function has a lot of parameters, you may want to rethink how you are splitting this up.

#### Rule #3. Refactoring your code: make your efficient code

##### (1) Reduce time complexity
##### (2) Reduce space complexity (memory/storage usage)

### 2. Documentation

#### Types of documentation
(1). In-line comments

(2). Function-level and Module-level comments (using Docstrings)

(3). Project-level comments: Your project should absolutely come with a README file. At a minimum, it should explain what it does, list its dependencies, and provide sufficiently detailed instructions on how to use it.


### 3. Version control in data science

Version control in data science can be tricky, because there are many pieces involved that can be hard to track, such as large amounts of data, model versions, seeds, hyperparameters, etc. Here are some resources for useful ways and tools for managing versions of models and large data.

(1). How to Version Control Your Production Machine Learning Models(https://algorithmia.com/blog/how-to-version-control-your-production-machine-learning-models)

(2). Version Control ML Model (https://towardsdatascience.com/version-control-ml-model-4adb2db5f87c)

### 4. Add robostness(reliablity) to your code
#### (1) Unit test

We want to test our functions in a way that is repeatable and automated. We can use unit test tool: PyTest. Have only one assert() statement per test

Test Driven Development Definition: Writing tests before you write the code that’s being tested.
Test driven development for data science is relatively new and has a lot of experimentation and breakthroughs appearing, which you can learn more about in the resources below.

-- Data Science TDD (https://www.linkedin.com/pulse/data-science-test-driven-development-sam-savage/)

-- TDD for Data Science (https://tanzu.vmware.com/content/pivotal-engineering-journal)

-- TDD is Essential for Good Data Science Here's Why (https://medium.com/uk-hydrographic-office/test-driven-development-is-essential-for-good-data-science-heres-why-db7975a03a44)

-- Testing Your Code (https://docs.python-guide.org/writing/tests/)

#### (2) Logging

Logging is the process of recording messages to describe events that have occurred while running your software. Let's take a look at a few examples, and learn tips for writing good log messages.

Tip #1: Be professional and clear

Tip #2: Be concise and use normal capitalization

Tip #3: Choose the appropriate level for logging

-- DEBUG - level you would use for anything that happens in the program.

-- ERROR - level to record any error that occurs

-- INFO - level to record all actions that are user-driven or system specific, such as regularly scheduled operations

Tip #4: Provide any useful information


#### (3) Code Review

-- Code review (https://github.com/lyst/MakingLyst/tree/master/code-reviews)

-- Code review best practice (https://www.kevinlondon.com/2015/05/05/code-review-best-practices.html)


