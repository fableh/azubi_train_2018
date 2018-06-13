
### Excercise 1.1 - Create the Device via SAP IoT Service

Open the SAP IoT Service cockpit by opening the following URL: 

https://sycor.eu10.cp.iot.sap/iot/cockpit/#

<img src="./img/cockpit.PNG" alt="cockpit" width="80%">

Login with the provided user and password.
And choose the "Devices" entry and  press the + icon to create a new device:

<img src="./img/create_device_01.PNG" alt="create device" width="80%">

In the upcoming screen specifiy your device:

| Property | Value |
| --- | --- |
| Name | e.g. Raspberry_PI_01 (identical to the user id from the cokpit user 'azubi_01')|
| Gateway | MQTT network (id = 2) |


<img src="./img/create_device_02.PNG" alt="create device" width="60%">

Congratulations! If the screen looks like this, u have successfully crated an Device on SAP IoT Services.

<img src="./img/create_device_03.PNG" alt="create device" width="60%">

The last step is now, to create a new "Sensor" an refer to an existing "Sensor Type" (for simplification the Sensor Type was created before).
To do this click again the + button and specify a new sensor:


| Property | Value |
| --- | --- |
| Name | e.g. MySensor |
| Sensor Type | CPU_SensorType |


<img src="./img/create_sensor.PNG" alt="create device" width="60%">
