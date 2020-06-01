Link Budget Report 

Considering that the satellite is placed in a 500 km orbit, we can calculate that the distance between the sat and a ground station, will be between 2000 km and 500 km as function of the elevation angle (5°- 90°)

Thus with this distance value, we can calculate the free space loss in best and worst cases. For a UHF Communication (440 Mhz) 

F@2000km = 151.3 dB 
F@500km   = 139.3 dB 

The modulations available to us are FSK, GMSK and ASK. But the ASK modulation does not allow for sufficiently good results. 

The recommended margins for a very low error rate (10^-8 %) for GMSK are 12dB and for FSK 15dB. 

It is therefore reasonable to take a signal-to-noise ratio margin of 15dB. 

On the satellite the availables performances are : 

Rx sensitivity from -100dB to -127 dB 
Tx Power up to 27dBm 
Antenna Gain from -25dB to 0dB 

On the ground : 

Rx sensitivity around -136dB
Tx Power up to 36dBm 
Antenna Gain from 10dB to 12dB 


Let’s start with the uplink; 

We transmit @36dBm with an antenna gain of 12dB ⇔ 48dB 
In best case we have a loss of -139.3 dB ⇔ 48+(-139.3) = - 91.3dB 
In worst case we have a loss of -151.3 dB ⇔ 48+(-151.3) = - 103.3 dB 

We have in best case an antenna with a 0dB Gain
Which mean that the power seen by the satellite is between - 91.3 dB and -103.3 dB 

We want a minimal signal-to-noise ratio margin of 15dB ⇔ -103.3 - 15 = - 118.3 dB 

Rx sensitivity on the sat should be better than - 118.3 dB 

Then Downlink; 

We transmit @27dBm with an antenna gain of 0dB ⇔ 27dB 
In best case we have a loss of -139.3 dB ⇔ 27+(-139.3) = - 112.3 dB 
In worst case we have a loss of -151.3 dB ⇔ 27+(-151.3) = - 124.3 dB 

We have an antenna gain around 12 dB on the ground station 
Which mean that the power seen by the ground station is between -100.3 and - 112.3 dB 

We want a minimal signal-to-noise ratio margin of 15dB ⇔ -112.3 - 15 = - 127.3 dB 

Rx sensitivity on the ground station should be better than - 127.3 dB 







