# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given an entry-card is issued for every new visitor, inclusing patients
  
  When a new patient arrives, an entry card is issued
  
  Then we compile results based on working days and holidays

Scenario: Compute parking slots to reserve for visiting specialists

  Given hospital staff attendance system and visit planned in advance
  
  When a specialist is to visit the hospital that day
  
  Then a parking slot is reserved for the specialist
