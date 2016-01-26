Objective:
This software is to simulate Surrey ADCS bundle. 


file input:
3 file required put in USB disk.
file name should be "ADCS_wx" "ADCS_wy" and "ADCS_wz".
each file contain one corresponding parameter, and the size of parameter is 2 
byte. (Big Endian)

I2c address: 0x02 (which should correct with 0x57)

I2c communication example:

write transfer: 0x92 (ID 146 Estimated Angular Rates)
read transfer: 0x11 0x11 0x22 0x22 0x33 0x33 (if system request 6 byte.)