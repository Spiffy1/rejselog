# Linter Setup

Developers should adopt and use linter because they provide a simple and effective way to improve the quality and consistency of their code. A linter is a tool that analyzes your code and reports any potential issues or inconsistencies, such as syntax errors, variable naming, code formatting, and more. By using a linter, developers can catch errors and mistakes early in the development process, which can save time and effort in the long run. Additionally, linter can help enforce coding standards and best practices, making it easier for developers to collaborate on projects and ensure code quality across the team. Overall, using a linter is a simple but powerful way for developers to write better, more consistent code and improve the overall quality of their projects.


## Code style - Black
Black should be included in the pipfile under the dev package If it isn't there, use 
```
pipenv install black --dev
```
- Go to File > Preferences > Settings on your Visual Studio Code IDE
- Then, search for “Formatting” and select “Format On Save”. 
- Make sure that this option is enabled and that the scope is on file only.

## Spelling Check - English literacy
Here are some of my recommendations:
1. Grammarly extension on VSC
2. Code Spell Checker extension on VSC.

## Import statements
- Your IDE should be able to detect unused import
- All imports should be grouped into 3 categories: built-in, library, local module
- Within each category, each module should be sorted based on the alphabet
For example:
```
import os
import sys

import pand
import scipy

import hotchili
from chili import pepper
from user import male
```

## Cognitive complexity (Sonarlint & Sonarqube)
Install Sonarlint from Visual Studio Code Extension (IDE)
Sonarqube server is a code analysis tool that can be installed locally and scan your project's code.

## Betterer
Betterer helps you keep track of certain stats, for example, line of code per function, unit test count, and warnings of any kind. This is best used in a pre-commit hook, where it will take a snapshot of all those numbers from your project and tell you which number gets better or worse. This tool is especially good for a large-scale project that involves many developers. 
```
https://phenomnomnominal.github.io/betterer/docs/introduction
```