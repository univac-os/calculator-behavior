# Multiplication

Scenario: Multiple of two positive numbers
  
  Given The calculator must be turn on

  When I type in "positive number"
       And I press "*"
       And I type in "positive number"
       And I press "equals"
  
  Then I see the "multiple number" as the result

Scenario: multiple of fraction
  
  Given The calculator must be turn on
  
  When I type in "fraction number"
  and I press "*"
  and I type in "fraction number"
  and I press "equals"
  
  Then I see the "multiple fraction number" as the result
  
Scenario: multiple of positive and negative number
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "*"
  and I type in "negative number"
  and I press "equals"
  
  Then I see the "negative number" as
  the result based on values
  
Scenario: Multiple of 1 
  
  Given The calculator must be turn on
  
  When I type in "number"
  and I press "*"
  and I type in "1"
  and I press "equals"
  
  Then I see the "same number" as the result

Scenario: Multiple of more than 2 numbers
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "*"
  and I type in "positive number"
  and I press "*"
  and till I press "equals"
  
  Then I see the "multiple positive number" as the result

Scenario: multiple numbers where the result goes out of range
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "*"
  and I type in "positive number"
  and I press "equals"
  
  Then I see the "ERROR" as the result if "added value" is
  more than certain value
  
Scenario: operation error
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "*"
  and I type in "another operator"
  and I press "positive number"
  and till I press "equals"
  
  Then I see the "multiple value with last sign
  stating operation taken" as the result
