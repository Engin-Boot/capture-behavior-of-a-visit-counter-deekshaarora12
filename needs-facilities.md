# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given the hospital is open,
  When
  Then

Scenario: Alert when seating capacity is full

  Given the hospital is open, a seat reading machine connected to a sensor
  When the user sits on the seat
  Then the sensor senses occupied seat,
  the seat reading machine records it, alerts with a red light when the seat
  capacity is full
