# GP proto CNC60100

Steps for configuring the software on a computer:

1. Activate .NET framework versions 3.5 and 4.7 in Windows, from **Turn Windows features on or off** menu.
1. Connect the machine
1. Install *UCCNC*, using the default `C:\UCCNC` directory. Do not open *UCCNC* yet
1. Copy the Profiles folder into the *UCCNC* folder
1. Copy the license file into the *UCCNC* folder
1. Right click on the desktop icon -> Property.
1. Change Destination string to `C:\UCCNC\UCCNC.exe /p GP010-1000`, so it defaults to the CNC60100 profile. 
1. Open UCCNC and start playing 

