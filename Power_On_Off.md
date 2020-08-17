
# Power-On and Power-Of

Scenario: User presses the power off button.

  Given the calculator is on
  
  When I press power button
  
  Then the calculator should be turned off and screen should be cleared.
  
Scenario: User presses the power on button.

  Given the calculator is off
  
  When I press power button
  
  Then the calculator should be turned on with clear screen.
