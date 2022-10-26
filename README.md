# 450V HV Indicator

![7873351665871968258](https://user-images.githubusercontent.com/14287399/197922667-3cffab45-05db-49bf-8a65-c0cddc485d22.png)


DESCRIPTION

This board (sponsored by JLCPCB) steps down our 450V battery pack voltage down to 12V, which then powers an LED to indicate that High Voltage has left our battery pack.

DETAILS

The HV Indicator board steps down 450V to 12V, using the LTC8316, an isolated Flyback converter.The indicator light is an LED on the accumulator that turns on whenever HV has left the accumulator, even when the accumulator is removed from the car. This is done for safety purposes, so people can tell when HV has left the accumulator. By FSAE competition rules, it must be directly powered by HV which is why a buck converter is directly tied to the 450V signal. The zener diode will not pass voltage below 39V, to make sure that when 39V+14V (minimum operating voltage for the buck) = 53V, the LED indicator light will turn on.

Key components:
  - LTC8316
  - 11328-T078

LTC8316

![8303961665871340232](https://user-images.githubusercontent.com/14287399/197922585-57ab786b-b6ca-4a69-ac2a-e860290c9f39.png)


Wide Input Voltage Range: 16V to 560V (600V max)

  - No Opto-Isolator Required for Regulation
  - Quasi-Resonant Boundary Mode Operation
  - Constant-Current and Constant-Voltage Regulation
  - Low-Ripple Light Load Burst Mode® Operation
  - Low Quiescent Current: 75μA
  - Programmable Current Limit and Soft-Start
  - High-Voltage Spacing

See more @https://www.analog.com/media/en/technical-documentation/data-sheets/lt8316.pdf

11328-T078: A transformer for HV and LV isolation on the board for safety and rules. The transformer splits up the majority of the HV sensing (done through the LT8316) from the diode and filtering around it, which is the portion of the board that is LV.

Features/Specifications:

  - Environmental RoHS compliant without exemption, REACH compliance
  - Operating temprature range: -40°C to 125°C (ambient + Temp rise)
  - Storage temperature range: -40°C to 125°C
