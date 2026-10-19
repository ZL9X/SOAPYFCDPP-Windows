# SOAPYFCDPP-Windows
A Windows SoapySDR driver for the FUNcube dongle pro+.

# What is this?
This is a Windows based SoapySDR driver for the FUNcube dongle pro+.  You can use it with any 64-bit Windows application that incorporates V.0.8 of the SoapySDR engine (it will not work with earlier versions).  It was developed for use in particular with SkyRoof by Alex Shovkoplyas, VE3NEA. 

https://ve3nea.github.io/SkyRoof/index.html 

# SkyRoof Installation

The dll file must be downloaded and then copied into the modules0.8 folder of your SkyRoof installation, usually C:\Program Files\Afreet\SkyRoof\lib\SoapySDR\modules0.8.

Plug in your Funcube to your PC and restart SkyRoof. You should see the Funcube as an option under Tools/SDR Devices".

The audio will need to be adjusted.  You have two options to set the audio:

1. Open Tools/SDR Devices. "Set "Single Gain" to "true" and use the RF Gain slider on the toolbar to set the audio (50-60 is a good starting point) or

2. Open Tools/SDR Devices. Set "Single Gain" to "false" and manually set the IF, LNA and Mixer settings (they are below Single Gain).  Start with LNA (max 10) and Mixer (max 20), IF (max 59).  Testing suggests LNA 10 Mixer 20 and IF 30 works well but it will depend on your antenna and noise level at your QTH.

If you change the LNA, Mixer and/or IF settings manually you will need to change the mode and then change it back to the one you want for the changes to take effect.  It is the same if you switch between true and false for "Single Gain".

If the waterfall looks noisy adjust contrast and brightness in the waterfall settings (button top left of waterfall screen).  Brightness 39 and contrast of 25 is a good starting point.  Don't forget to use the mouse wheel to zoom in on the display so you can see the satellite carriers (and your noise level).     

# Download

https://github.com/Zl9x/SOAPYFCDPP-Windows/releases/tag/v1.0.0
