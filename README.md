# GPSrx
##Reception of GPS signals from RTL-SDR and getting raw GPS data
* Using GNU radio software to realize the incoming data and plot its spectrum.
* GPS signals are well below the thermal noise, but can be received because it uses C/A signals which uses Spectrum spreading using PRN (Pseudo Random) Codes.
* By correlating the received signal (which looks like noise) by the C/A PRN code, GPS receivers receive data from satellites

##Results
* How PRN gold codes look like?, here are g5 and g17 C/A codes
  ![Img](https://raw.githubusercontent.com/ajinkyagorad/GPSrx/master/img/PRNgcode.jpg)
* Correlation with USRP data for 37 C/A codes
  ![Img](https://raw.githubusercontent.com/ajinkyagorad/GPSrx/master/img/37CAcodeCorr.jpg)
* Under simulated noise conditions, from SNR of -20dB to 0dB, input attenuated, with 5 same cacode
  ![Img](https://raw.githubusercontent.com/ajinkyagorad/GPSrx/master/img/sim_noise_attn.jpg)

####Things to do next!!!
* -[ ] what exactly is the format of GNUradio .bin file?
* -[x] check the CA code correlation on the simulated noise!
