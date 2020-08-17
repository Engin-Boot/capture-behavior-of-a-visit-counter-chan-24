# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given A calendar and a sensor(entry card issuer)
  When Patient gets in on working days/ holidays
  Then Give entry cards of blue colors/ red colors

Scenario: Compute parking slots to reserve for visiting specialists

  Given Number of available parking slots and number of incoming
  visiting specialists on a particular day
  When Number of available parking slots becomes equal to
  number of incoming visiting specialists  on a particular day yet to arrive
  Then Do not allow others to park in the parking area
