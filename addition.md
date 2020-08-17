# Addition

Scenario: Addition of two positive integer numbers
  
  Given the calculator is turned on and the calculator screen is clear.

  When I type in positive number
        And press plus
        And type in poisitive number
        And press equals.
  
  Then Calculator screen will show addition of two positive numbers.


Scenario: Addition of two negative numbers.
  
  Given the calculator is turned on and the calculator screen is clear.

  When I type in negative number
        And press plus
        And press opening bracket
        And type in negative number
        And press closing bracket
        And press equals.
  
  Then Calculator screen will show addition of two negative numbers.
  
 
Scenario: Addition of one positive and one negative numbers.
  
  Given the calculator is turned on and the calculator screen is clear.

  When I type in positive number
        And press plus
        And press opening bracket
        And type in negative number
        And press closing bracket
        And press equals.
  
  Then Calculator screen will show addition of two numbers.
  
 
Scenario: Addition of one negative and positive numbers.
  
  Given the calculator is turned on and the calculator screen is clear.

  When I type in negative number
        And press plus
        And type in positive number
        And press equals.
  
  Then Calculator screen will show addition of two numbers.
 
 
Scenario: Addition of more than two numbers.
  
  Given the calculator is turned on and the calculator screen is clear.

  When I type in number
        And press plus
        And type in another number
        And press plus
        And type in another number
        And repeat press plus and type in another number for remaining numbers
        And press equals.
  
  Then Calculator screen will show addition of all the numbers.
  
  
Scenario: Addition of two decimal numbers.
  
  Given the calculator is turned on and the calculator screen is clear.

  When I type in decimal number
        And press plus
        And type in decimal number
        And press equals.
  
  Then Calculator screen will show addition of two decimal numbers.
  
  
Scenario: Addition of numbers where result goes out of range.
  
  Given the calculator is turned on and the calculator screen is clear.

  When I type in number
        And press plus
        And type in number
        And press equals.
  
  Then Calculator will show addition out of range on calculator screen.
  
    
Scenario: When input syntax is invalid.
  
  Given the calculator is turned on and the calculator screen is clear.

  When I type in number
        And press plus
        And type in number
        And 
        And press equals.
  
  Then Calculator will show invalid syntax on calculator screen.
  
 
Scenario: When plus operator is pressed more than once successively.
  
  Given the calculator is turned on and the calculator screen is clear.

  When I type in number
        And press plus
        And press plus
        And type in number
        And press equals.
  
  Then Calculator will show invalid syntax on calculator screen.
  
Scenario: Addition of two fractions.
  
  Given the calculator is turned on and the calculator screen is clear.

  When I press opening bracket
        And type in fraction
        And closing bracket
        And press plus
        And press opening bracket
        And type in fraction
        And closing bracket
        And press equals.
  
  Then Calculator screen will show addition of fractions.
