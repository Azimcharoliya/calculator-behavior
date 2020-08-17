
# Power-On and Power-Of

Scenario: User presses the power off button.

  Given the calculator is on
  
  When I press power button
  
  Then the calculator turns off and screen clears.
  
Scenario: User presses the power on button.

  Given the calculator is off
  
  When I press power button
  
  Then the calculator turns on with clear screen.
