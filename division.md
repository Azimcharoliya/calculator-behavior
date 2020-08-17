# Division

Scenario: Division of two positive integer numbers
  
  Given the calculator is on and the calculator screen is clear.

  When I type in positive number\
        And press divide\
        And type in positive number\
        And press equals.
  
  Then the calculator screen will show division of two positive numbers.

Scenario: Division of two negative numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in negative number\
        And press divide\
        And press opening bracket\
        And type in negative number\
        And press closing bracket\
        And press equals.
  
  Then the calculator screen will show division of two negative numbers.
  
Scenario: Division of one positive and one negative numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in positive number\
        And press divide\
        And press opening bracket\
        And type in negative number\
        And press closing bracket\
        And press equals.
  
  Then the calculator screen will show division of two numbers.
  
Scenario: Division of more than two numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in number\
        And press divide\
        And type in another number\
        And press divide\
        And type in another number\
        And repeat press divide and type in another number for remaining numbers\
        And press equals.
  
  Then the calculator screen will show division performed in right to left manner.

Scenario: Division of two decimal numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in decimal number\
        And press divide\
        And type in decimal number\
        And press equals.
  
  Then the calculator screen will show division rounded upto two decimal places.
  
Scenario: When input syntax is invalid.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in number\
        And press divide\
        And type in number\
        And press divide\
        And press equals.
  
  Then the calculator will show invalid syntax on calculator screen.

Scenario: division of two fractions.
  
  Given the calculator is on and the calculator screen is clear.

  When I press opening bracket\
        And type in fraction\
        And closing bracket\
        And press divide\
        And press opening bracket\
        And type in fraction\
        And closing bracket\
        And press equals.
  
  Then the calculator screen will show division of fractions.
  
Scenario: Division of numbers where result goes out of range.

  Given the calculator is on and the calculator screen is clear.

  When I type in number\
        And press divide\
        And type in number\
        And press equals.

  Then the calculator will show out of range on calculator screen.

Scenarios: Pressing divide button more than one times.

  Given the calculator is on and the calculator screen is clear.

  When I type in number\
        And press divide\
        And press divide again\
        And type in number\
        And press equals.

  Then the calculator will show division on calculator screen.
  
Scenarios: Division by one.

  Given the calculator is on and the calculator screen is clear.

  When I type in first number\
        And press divide\
        And type in 1\
        And press equals.

  Then the calculator screen will show the first number.
  
Scenarios: Division by zero when operand one is any number.

  Given the calculator is on and the calculator screen is clear.

  When I type in first number\
        And press divide\
        And type in 0\
        And press equals.

  Then the calculator will show can't divide by zero on calculator screen.
  
Scenarios: Division zero by any number except zero.

  Given the calculator is on and the calculator screen is clear.

  When I type in 0\
        And press divide\
        And type in number\
        And press equals.

  Then the calculator will show zero on calculator screen.
  
Scenarios: Recurring decimal case.

  Given the calculator is on and the calculator screen is clear.

  When I type in number\
        And press divide\
        And type in number \
        And press equals.

  Then the calculator screen will show the division
  with line drawn over a recurring pattern.
