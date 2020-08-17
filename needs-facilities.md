# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given Data of visitors in a week
  When Many visitors do not have meals in hospital canteen
  Then Reduce the number of meals prepared in canteen in the next week

Scenario: Alert when seating capacity is full

  Given Total number of seats and visitor count
  When A new visitor enters and visitor count equals number of seats
  Then Alert the staff for alternate arrangement
