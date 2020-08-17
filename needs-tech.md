# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given the visit-counter
  
  When the server restarts
  
  Then visitor counter becomes zero

Scenario: Reconcile counts if the sensor is offline for a while

  Given a visit-counter sensor
  
  When the sensor goes offline for a while
  
  Then the counter re-starts from the last counter value
