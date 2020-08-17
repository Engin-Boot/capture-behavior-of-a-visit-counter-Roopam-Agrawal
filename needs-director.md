# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given an entry-card, for every new visitor including patients
  
  When a new patient arrives, issue an entry card
  
  Then we compile results based on working days and holidays

Scenario: Compute parking slots to reserve for visiting specialists

  Given hospital staff attendance system and planned visit by specialist
  
  When a specialist is to visit the hospital that day
  
  Then reserve a parking slot for the specialist
