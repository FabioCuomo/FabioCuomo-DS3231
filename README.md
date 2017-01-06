# FabioCuomo-DS3231
A modified arduino library for DS3231 RTC

This is a fork of the Adafruit library https://github.com/adafruit/RTClib, which I extended for DS3231 only by integrating some additional commands found in Jack Christensen's library https://github.com/JChristensen/DS3232RTC.
I added commands for reading temperature and for using DS3231 alarms, that I needed for implementing wake-up of arduino on interrupt after entering the sleep state.

Update 06-Jan-2017

Added functions for reading and writing bytes on DS3231 memory control registers: 
- byte read(byte addr);
- void write(byte addr, byte value);
