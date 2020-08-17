# Addition

Scenario: Addition of two positive numbers
  
  Given The calculator must be turn on

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
  
Scenario: Addition of postive and negative number
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "plus"
  and I type in"negative number"
  and I press "equals"
  
  Then I see the "postive number" as the result if psotive number is more than negative number 
  or I see the "nagative number" as the result in vice versa conditon

Scenario: Addition of decimals
  
  Given The calculator must be turn on
  
  When I type in "decimal number"
  and I press "plus"
  and I type in"decimal number"
  and I press "equals"
  
  Then I see the "added decimal number" as the result

Scenario: Addition of fraction
  
  Given The calculator must be turn on
  
  When I type in "fraction number"
  and I press "plus"
  and I type in"fraction number"
  and I press "equals"
  
  Then I see the "added fraction number" as the result

