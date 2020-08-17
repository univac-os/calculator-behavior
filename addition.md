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
  and I type in "fraction number"
  and I press "equals"
  
  Then I see the "added fraction number" as the result
  
Scenario: Addition of positive and negative number
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "plus"
  and I type in "negative number"
  and I press "equals"
  
  Then I see the "positive/neagtive number" as 
  the result based on values
  
Scenario: Addition of decimals
  
  Given The calculator must be turn on
  
  When I type in "decimal number"
  and I press "plus"
  and I type in "decimal number"
  and I press "equals"
  
  Then I see the "added decimal number" as the result

Scenario: Addition of more than 2 numbers
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "plus"
  and I type in "positive number"
  and I press "plus"
  and till I press "equals"
  
  Then I see the "added positive number" as the result

Scenario: Adding numbers where the result goes out of range
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "plus"
  and I type in "positive number"
  and I press "equals"
  
  Then I see the "ERROR" as the result if "added value" is
  more than certain value
  
Scenario: operation error
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "plus"
  and I type in "another operator"
  and I press "positive number"
  and till I press "equals"
  
  Then I see the "ERROR stating operation error" as the result
  
