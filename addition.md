# Addition

Scenario: Addition of two positive numbers
  
  Given The calculator must be turns on

  When I type in "positive number"
       And I press "plus"
       And I type in "positive number"
       And I press "equals"
  
  Then I see the "added number" as the result

Scenario: Addition of fraction
  
  Given The calculator must be turn on
  
  When I type in "fraction number"
  and I press "plus"
  and I type in"fraction number"
  and I press "equals"
  
  Then I see the "added fraction number" as the result
