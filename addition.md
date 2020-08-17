# Addition

Scenario: Addition of two positive numbers
  
  Given The calculator must be turns on

  When I type in "positive number"
       And I press "plus"
       And I type in "positive number"
       And I press "equals"
  
  Then I see the "added number" as the result

Scenario: (describe a scenario here)
  
  Given (state the initial condition)
  
  When (state the event)
  
  Then (state the effect)
