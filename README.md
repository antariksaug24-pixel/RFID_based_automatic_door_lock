# RFID_based_automatic_door_lock

Components Used
The system employs an Arduino Microcontroller, an RFID Reader, and several other components which are detailed below:
Arduino: This acts as the brain of the system. It receives signals from the RFID reader, processes them, and subsequently sends commands to either grant or deny access.
LCD Display: This display module offers feedback to the user. It can showcase messages such as “Access Granted”, “Access Denied”, or “Scan your RFID card”.
RFID Reader: This component reads the RFID card or tag presented by the user. If the RFID data aligns with the stored information, it sends a signal to the Arduino for further action. The RC522 SPI Module is the most popular module in the market which has been used in this project.
LED Indicator: This provides visual feedback about the system’s status. For instance, a green LED might indicate successful access, while a red LED could signify denied access.
Buzzer: An auditory component that can sound alerts or notifications based on the system’s status or user interactions.
Relay: This electrically operated switch is activated when the Arduino sends a command to grant access.
Solenoid Lock: An electronic lock mechanism that can be locked or unlocked when powered. The relay, when activated, supplies power to this lock, causing it to unlock.
System Operation
The RFID Based Door Lock Security System is engineered to offer secure access control through RFID card verification. Central to the system are an RFID reader, an Arduino microcontroller, a relay, a solenoid lock, an LCD display, an LED indicator, and a buzzer. Users mainly interact with the system by presenting their RFID cards to the reader and receiving feedback via the LCD display and LED indicator.
When a user scans their RFID card, the reader captures the card’s data and forwards it to the Arduino for validation. The Arduino then compares this data with the stored RFID information. If there’s a match, the Arduino triggers the relay, which subsequently powers the solenoid lock, unlocking it. Throughout this procedure, the LCD display and LED indicator provide real-time feedback to the user, indicating actions required or the outcome of the verification, such as “Access Granted” or “Access Denied”.
Circuit Diagram of RFID Door Lock Security System using Arduino
For the Power Supply unit, the entire device is powered using a 12V DC Power Adapter. The 7805 Voltage regulator IC power the Relay and relay using the 5V output of the 7805 regulator. The 12V Supply is also connected to the Vin Pin of Arduino Nano. The 100uF/35V Electrolytic Capacitor is used for Voltage Stability at Power Supply Pins.