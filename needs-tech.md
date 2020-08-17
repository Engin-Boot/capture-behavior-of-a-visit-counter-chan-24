# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given the server running visit-counter 
  is restarting
  When a new visitor is trying to enter 
  Then stop the visitor from entering 
  till server finishes restarting
  
Scenario: Reconcile counts if the sensor is offline for a while

  Given the sensor is offline for a while
  When a visitor enters 
  Then make arrangements for alternate counting 
  and add this to sensor before sensor comes online again
