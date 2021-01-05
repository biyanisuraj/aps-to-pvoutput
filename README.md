# aps-to-pvoutput
Upload data from AP Systems solar inverters (APS) automatically to PV Output

Install this script for example on a Raspberry PI and schedule crontab to run it every 5 minutes!

# How to install?

## Make an account
@ [PV output](https://pvoutput.org)

## Create/Upload Script
Than just created a new script within `Domoticz/scripts/python`:

```
cd domoticz/scripts/python
sudo nano apstopvoutput.py
```

- Copy code from `apstopvoutput.py` and paste it into the `apstopvoutput.py` file

- change the things below in in the script. Leave the ' ' and replace the (for example) <ecuid> with the corresponding data

```
ECU_ID = '<ecuid>'
PV_OUTPUT_SYSTEMID = '<systemid>'
PV_OUTPUT_APIKEY = '<apikey>'
```

> you can find the *ECU id* in your app for example. The *PV_OUTPUT_SYSTEMID and APIKEY* you can find @ pvoutput.org

exit the file with Crtl-X and than save with Y(es) and confirm with enter

Than just follow the pvoutput guide (https://www.domoticz.com/wiki/Domoticz_and_PvOutput.org) to get the pvoutput data in your domoticz.
