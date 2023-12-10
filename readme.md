# Open3E-HA 

In this repository I would like to collect information that is needed for the integration of Open3E in Home Assistant. 

    https://github.com/abnoname/open3e

Further information can be found here: 

    https://github.com/abnoname/open3e/discussions/54

    https://www.viessmann-community.com/t5/Konnektivitaet/CAN-Bus-Home-Automation-E3-Generation-lokal-und-kostenlos/td-p/356066

At the moment I have limited myself to a few data points to illustrate the principle. I start the Open3E client with the following call: 

    python3 Open3Eclient.py -c can0 -dev vcal -r 268,269,274,284,286,318,320,321,322,324,325,381,401,402,475,476,880,881,901,902,987,988,1415,1416,1643,1644,2346,2351,2352,2369,2370,2487,2569 -v -muser MyHaUsername:MyHaPassword -m 192.168.xxx.xxx:1883:open3e -mfstr "{didNumber}_{didName}" -t 30

I then have the data points in the MQTT server with this structure:

    open3e/274_OutsideTemperatureSensor/Actual

