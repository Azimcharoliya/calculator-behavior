# Subtraction

Scenario: Subtraction of two positive integer numbers
  
  Given the calculator is on and the calculator screen is clear.

  When I type in positive number\
        And press minus\
        And type in positive number\
        And press equals.
  
  Then Calculator screen will show subtraction of two positive numbers.

Scenario: Subtraction of two negative numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in negative number\
        And press minus\
        And press opening bracket\
        And type in negative number\
        And press closing bracket\
        And press equals.
  
  Then Calculator screen will show subtraction of two negative numbers.
  
Scenario: Subtraction of one positive and one negative numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in positive number\
        And press minus\
        And press opening bracket\
        And type in negative number\
        And press closing bracket\
        And press equals.
  
  Then Calculator screen will show subtraction of two numbers.
  
Scenario: Subtraction of one negative and positive numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in negative number\
        And press minus\
        And type in positive number\
        And press equals.
  
  Then Calculator screen will show subtraction of two numbers.

Scenario: Subtraction of more than two numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in number\
        And press minus\
        And type in another number\
        And press minus\
        And type in another number\
        And repeat press minus and type in another number for remaining numbers\
        And press equals.
  
  Then Calculator screen will show subtraction of all the numbers.

Scenario: Subtraction of two decimal numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in decimal number\
        And press minus\
        And type in decimal number\
        And press equals.
  
  Then Calculator screen will show subtraction of two decimal numbers.
  
Scenario: When input syntax is invalid.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in number\
        And press minus\
        And type in number\
        And press minus\
        And press equals.
  
  Then Calculator will show invalid syntax on calculator screen.

Scenario: Subtraction of two fractions.
  
  Given the calculator is on and the calculator screen is clear.

  When I press opening bracket\
        And type in fraction\
        And closing bracket\
        And press minus\
        And press opening bracket\
        And type in fraction\
        And closing bracket\
        And press equals.
  
  Then Calculator screen will show subtraction of fractions.
