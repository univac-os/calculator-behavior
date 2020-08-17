# Multiplication

Scenario: Multiple of two positive numbers
  
  Given The calculator must be turn on

  When I type in "positive number"
       And I press "*"
       And I type in "positive number"
       And I press "equals"
  
  Then I see the "positive multipled number" as the result

Scenario: multiple of fraction
  
  Given The calculator must be turn on
  
  When I type in "fraction number"
  and I press "*"
  and I type in "fraction number"
  and I press "equals"
  
  Then I see the "multipled fraction number" as the result
  
Scenario: multiple of positive and negative number
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "*"
  and I type in "negative number"
  and I press "equals"
  
  Then I see the "negative number" as
  the result based on values
  
Scenario: multiple of 0

  Given The calculator must be turn on
  
  When I type in "number"
  and I press "*"
  and I type in "0"
  and I press "equals"
  
  Then I see the "zero" as the result

Scenario: Multiple of more than 2 numbers
  
  Given The calculator must be turn on
  
  When I type in "positive number"
  and I press "*"
  and I type in "positive number"
  and I press "*"
  and till I press "equals"
  
  Then I see the "multipled positive number" as the result

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
  
  Then I see the "multipled value with last sign
  stating operation taken" as the result
