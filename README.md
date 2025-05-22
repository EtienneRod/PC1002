For more information how to configure in home assistant look at https://community.home-assistant.io/t/hayward-oasis-and-other-generic-pool-heatpump-using-pc1002/733827/30

To resume, you need to connect RS485 to CN3, pinout is from right to left +12V, RS485_A, RS485_B, GND. Don't forget that you need to rollover (cross cronnect) A and B from the CN3 connector to your RS485 gateway so RX is connected to TX.

After, add all lines included in configuration_hayward.yaml to the mqttt section (create it if not existent) in configuration.yaml of your home assistant. Also, create an automation and paste all yaml included in on_off_automation.yaml
