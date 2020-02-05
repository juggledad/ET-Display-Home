# ET-Display-Home
Node-RED manager for ESPEasy, Sonoff/Tasmota and Homie flashed devices 

When INSTALLING FOT THE FIRST TIME" go to the initialization tab and run 'STEP 2' to build the SQLite database/table.

This flow first gets the IP range of your network. It then checks for the latest versions of ESPEasy, Sonoff/Tasmota and Homie to display and provide a link to download the version.

It then proceeds to scan your network looking for ESPeasy, Tasmota or Homie flashed devices. For each one it finds, it stores them in the database. It also store wether they are ON or OFF line. Finally they are stored in a database for future access.

There is also a section on the dashboard that will allow you to delete 'ghost' devices by IP address. 'Ghost' devices occur when you flash a device and it is assigned an IP address and that device is found and stored in the database. Subsequently you change the IP address of the device. The original database entry exists and is now a 'ghost'.
