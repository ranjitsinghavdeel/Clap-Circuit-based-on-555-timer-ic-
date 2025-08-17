# Clap_Circuit_based_on_555_timer_ic
The proposed Clap circuit is designed to function as a automatic light switching circuit based on a high decibel clap from user. The system uses LM393 Sound sensor which in coordination with 555 timer ic is connected to make the system. The 555 timer ic is used in monostable state to keep the system running infinitely.
# Tech Stack
Hardware:
1) LM393 Sound sensor module
2) 555 Timer ic
3) LED
4) Push button
5) Resistors ( 220 ohm, 1 k ohm)
6) 9 V battery
# Working 
- The clap circuit works by giving a high decibel input(by clapping) to the LM393 sound sensor which can detect this audio signal and convert it into digital signals.
- When a clap is detected LM393 gives a low digital signal to 555 timer ic via pin 2, which triggers the ic to start its timer cycle.
- 555 timer ic is connected in monostable state which means it will keep the circuit in high state as long as its timer is running.
- This high signal is then given to LED using pin 3 of 555 ic which turns the LED on till the 555 timer ic is working.
- To stop the 555 timer ic’s timer cycle a push button is used to reset the circuit by temporarily shutting the power supply.
# circuit connections
- LED is connected to GND via 220 ohm resistor and its anode is connected to the 3 pin (OUTPUT) of 555 timer ic.
- Push Button(S1) is connected to GND and other pin is connected to Vcc and anode of LED. 
- 555 timer ic’s pin 1(GND) is connected to GND, pin 2(Trigger) connected to LM393 D0 pin(digital output pin). pin 3(OUT) is connected to LED, pin 8(Vcc) and pin 4(reset) connected to each other, pin 7(discharge) and pin 6(threshold) connected to each other.
- LM393 pin D0 connected to pin 2 of 555 timer ic, pin + connected to Vcc and pin G connected to GND.
# Results
- The given circuit can successfully detect audio inputs from user.
- The proposed system can successfully turn on a LED by detection of a clap.
- The system can reset using a push button, therefore allowing user to switch off LED when needed.
- The system is cost-effective and easy to install in a real-life scenario, but will require relay, voltage divider, AC-DC adapter, rectifier, etc.
