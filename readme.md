# Open3E-HA 

In this repository I would like to collect information that is needed for the integration of Open3E in Home Assistant. 

    https://github.com/abnoname/open3e

Further information can be found here: 

Installation instructions: [Installation](./installation.md)

    https://github.com/abnoname/open3e/discussions/54

    https://www.viessmann-community.com/t5/Konnektivitaet/CAN-Bus-Home-Automation-E3-Generation-lokal-und-kostenlos/td-p/356066

I start the Open3E client with the following call: 

    python3 Open3Eclient.py @../args.txt

    -> args.txt : The following values must be adjusted: --mqtt (ip), --mqttuser (username and password)

I then have the data points in the MQTT server with this structure:

    open3e/680_274_OutsideTemperatureSensor/Actual

In HA, I have created a folder "packages", which then contains the `vitocal250.yaml` files.

A complete installation guide is here: [installation.md](installation.md)

