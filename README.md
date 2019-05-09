# PCB files for Adafruit MAX31850 1-Wire Thermocouple Breakout Board

<a href="http://www.adafruit.com/products/1727"><img src="assets/image.jpg?raw=true" width="500px"><br/>Click here to purchase one from the Adafruit shop</a>

Thermocouples are very sensitive, requiring a good amplifier with a cold-compensation reference. [So far we've carried the very nice MAX31855 which is an SPI interface thermocouple amplifier](https://www.adafruit.com/products/269). The '855 is great but if you have a lot of thermocouples to measure it isn't terribly easy to use. That's why we are also carrying the new '850 model from Maxim - it's a "1-Wire" thermocouple amp which can have any number of breakouts on a single shared I/O line.

The MAX31850K does everything for you, and can be easily interfaced with any microcontroller that has 1-Wire support. This breakout board has the chip itself, a 3.3V regulator with 10uF bypass capacitors all assembled and tested. This board can be used with 'parasitic power' - where the power is on the data line - or with 'local power' where the power for the converter comes in on the Vin Pin.

Please note: this board does not have level shifting on the 3V Data line - we did this on purpose so that it can be used in parasitic mode. The data line must be level shifted to [3V - our 4-channel shifter works wonderfully for level shifting 1-Wire](http://www.adafruit.com/products/757) and you only need one at the '1-Wire host' for all thermocouples on the shared data line.

The MAX31850K data format is very similar to that of the well known 1-Wire DS18B20 temp sensor but it is not drop in compatible without code changes to check for the new '1 Wire family' type. We have adapted the classic Arduino [OneWire](https://github.com/adafruit/MAX31850_OneWire) and [DallasTemp](https://github.com/adafruit/MAX31850_DallasTemp) libraries to be MAX31850 compatible, so please click on those links to grab our libraries.

Comes with a 2 pin terminal block (for connecting to the thermocouple), 4.7K data line pullup resistor, and pin header (to plug into any breadboard or perfboard).
[Goes great with our 1m K-type thermocouple](http://www.adafruit.com/products/270). Not for use with any other kind of thermocouple, K type only!<Paste>

- Works with any K type thermocouple
- Will not work with any other kind of thermocouple other than K type
- -270C to +1370C output in 0.25 degree increments
- Internal temperature reading
- 3.3 to 5v power supply. Data line is 3V only
- 1-Wire interface allows any number of thermocouple amps on a single data line

Note: The terminal block included with your product may be blue or black.

## License

Adafruit invests time and resources providing this open source design, 
please support Adafruit and open-source hardware by purchasing 
products from Adafruit!

Designed by Limor Fried/Ladyada for Adafruit Industries.
Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution
All text above must be included in any redistribution
