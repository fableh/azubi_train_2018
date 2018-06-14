### Excercise 2 - Build up the Digital Twin with SAP Cloud Platform IoT Application Enabalmenet

#### Login to SAP CP IoT Application Enablment

Please enter the SAP Cloud Platform IoT Application Enablment:

[SAP CP IoT AE](https://sycor-cf-subaccount.iot-sap.cfapps.eu10.hana.ondemand.com/launchpage/index.html#Shell-home)

Enter your credentials an "Log on":

<img src="./img/login.PNG" alt="login" width="60%">

Afterwards you can see the initial launchpad, press now the Package Manager tile to enter the application:

<img src="./img/flp.PNG" alt="login" width="60%">

Now search the "syc.azubi.train" package:

<img src="./img/package01.png" alt="package" width="60%">

And click on the follwing button to display the "Property Sets":

<img src="./img/package02.png" alt="enter the property sets" width="60%">

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

Save yor changes and switch over to the "Thing Modeler" by pressing the link in the lower right corner:

<img src="./img/TM_SWITCH.PNG" alt="package" width="60%">




