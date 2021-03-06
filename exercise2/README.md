### Excercise 2 - Build up the Digital Twin with SAP Cloud Platform IoT Application Enabalmenet

#### Login to SAP CP IoT Application Enablment

Please enter the SAP Cloud Platform IoT Application Enablment:

[SAP CP IoT AE](https://sycor-cf-subaccount.iot-sap.cfapps.eu10.hana.ondemand.com/launchpage/index.html#Shell-home)

The offical SAP Help documentation can be found here:

[SAP Help](https://help.sap.com/viewer/p/SAP_IOT_APPLICATION_SERVICES)

Enter your credentials an "Log on":

<img src="./img/login.PNG" alt="login" width="40%">

Afterwards you can see the initial launchpad, press now the Package Manager tile to enter the application:

<img src="./img/flp.PNG" alt="login" width="60%">

Now search the "syc.azubi.train" package:

<img src="./img/package01.png" alt="package" width="60%">

And click on the follwing button to display the "Property Sets":

<img src="./img/package02.png" alt="enter the property sets" width="60%">

#### Creat a new Property Set

As u can see there are 2 property sets available:

<img src="./img/ps.PNG" alt="package" width="60%">

Please familarize with CPU "Property Set" (PS) this is pre- created and will be used for the Thing configuration.

In the next step u can create now an own PS e.g. for some Basic informations, feel free an define your own.

Based on the fact that these package is used together, it make sense also here to use an identifier.

<img src="./img/new_ps.PNG" alt="creat a new property set" width="60%">

You can finally spcefiy some fields e.g.:

| Property | Type |
| --- | --- |
| Product | String |
| Last Maintenance | Date |
| Color | String |
| ... | ... |

#### Create a new Thing Type

Save yor changes and switch over to the "Thing Modeler" by pressing the link in the lower right corner:

<img src="./img/TM_SWITCH.PNG" alt="package" width="40%">

Afterwards creat a new Thing Type:

<img src="./img/CREATE_NEW_TT.PNG" alt="package" width="40%">

By pressing the + button in the "Basic Data" section should link now yor previous created property set:

<img src="./img/LINKPS.PNG" alt="package" width="40%">

Futhermore link the CPU property set under "Measured Values" and upload an image of your choice for your thing.

As result the final Thing Type looks now like this, which has now two linked property sets:

<img src="./img/CREATE_RPI_THING.PNG" alt="package" width="80%">

#### Create a new Thing

To bind our real "IoT Device" the Raspberry PI to our newly created Thing Type we need to create an new Thing.
This Thing is the virtual representaion ans has 1:1 relationship to our SAP IoT service type.

<img src="./img/DATA_MODEL_MAPPING.PNG" alt="package" width="80%">

You start the creation process for our Thing by pressing the "new Thing" button in the upper left corner.

<img src="./img/NEW_THING.PNG" alt="package" width="40%">

#### Connect booth Worlds

In the upcomming screen you can now connect your real device with the previously created Thing Type.

First specify the Basic Data for your Thing:

<img src="./img/BASIC_DATA_THING.PNG" alt="package" width="40%">

Bind the IoT Service Device (pls verify that u use the right "your" Device ID):

<img src="./img/DEVICE_ID.PNG" alt="package" width="40%">

Sensor ID:

<img src="./img/SENSOR_ID.PNG" alt="package" width="40%">

If u has done all steps before correct you should now see a "green" mapping:

<img src="./img/MAPPING.PNG" alt="package" width="40%">

And finally u got the unique Thing ID:

<img src="./img/RESULT.PNG" alt="package" width="40%">

#### Verify the incoming data

If u now check the new Thing you are able to enter the basic data:

<img src="./img/THING_BASIC_DATA.PNG" alt="package" width="60%">

And under the measured values u are able to see now the incoming data:

<img src="./img/INCOMING_DATA.PNG" alt="package" width="60%">

#### Send data back to the device

As in Excercise 1 introduced we are using the [MQTT](http://mqtt.org/) protocol, which allows us to send data bi-directional.
If u now open the tree where u see the incoming data, u can also type in a value and click save.

<img src="./img/SEND_DATA_BACK.PNG" alt="package" width="60%">

Please switch back to the terminal where u are connected to the raspberry and u can see the data is there:

<img src="./img/INCOMING_AT_DEVICE.PNG" alt="package" width="60%">

Congratulations! you are successfuly finished the second excercise !!!

Start here with [Exercise3](../exercise3/README.md)







