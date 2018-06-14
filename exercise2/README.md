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

<img src="./img/THINGTYPE.PNG" alt="package" width="40%">

By pressing the + button in the "Basic Data" section should link now yor previous created property set:

<img src="./img/LINKPS.PNG" alt="package" width="40%">

Futhermore link the CPU property set under "Measured Values" as result the final Thing Type looks now like this:

<img src="./img/FINAL_TT.PNG" alt="package" width="60%">

#### Create a new Thing
