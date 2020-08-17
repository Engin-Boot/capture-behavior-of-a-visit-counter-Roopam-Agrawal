# Visit-counter for a Facilities Manager 

Scenario: Report visitor trends during a week of operation

  Given a foot-fall counter at the door

  When any new visitor enters the hospital, we increment the visitor counter
  
  Then we compile the visitor trends during the week

Scenario: Alert when seating capacity is full

  Given an entry-card issuer sensor
  
  When the current issued number of visitor cards is equal to the seating capacity 
  
  Then alert that the seating capacity is full 
