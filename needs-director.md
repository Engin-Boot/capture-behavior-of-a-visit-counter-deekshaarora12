# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given the hospital is open and a voice assistant which issues a token
  When the patient registers his name using the voice assistant
  And gets a token
  Then the token shows the number representing patient count
  updated by voice machine reported to the director

Scenario: Compute parking slots to reserve for visiting specialists

  Given the hospital is open and a card reading machine with a specialist QR-card
  When the car enters the parking
  And the card reading machine reads the card of specialist
  Then it displays a red light for specialist and green light
  for patient updates the slot filled and reports to the director
