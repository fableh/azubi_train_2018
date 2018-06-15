
### Excercise 3 - Visualize the IoT Data by develoing an SAPUI5 Application with SAP Web IDE

#### Open SAP Web IDE

We want cover now in this Excercise, how we can developing an simple SAP UI5 Application to visualize our IoT Data.

As u can see in the picture, SAP Application Enablement provides different tools to support the developer ecperience:

<img src="./img/IOT_AE_DEV_EXP.PNG" alt="create device" width="80%">


Please enter the SAP Web IDE (depending on the bandwith this can be took a while)

[SAP Web IDE](https://webidecp-a57d428ce.dispatcher.hana.ondemand.com)

Futher Informations about SAP Web IDE and the available Controls for SAP Web IDE in the context with SAP IoT Application Enablmenet:

[SAP Help](https://help.sap.com/viewer/825270ffffe74d9f988a0f0066ad59f0/Cloud/en-US/0221845d73ad403ab2852142f3179177.html)

[SAP IoT Application Enablement Developer Guide](https://help.sap.com/viewer/53368b9f996c42fda75faccf5e986873/1.57.0.0/en-US)

#### Familarize with the SAP Web IDE and check the Plugin

After the successfully start of the SAP Web IDE, you should see an empty workspace:

<img src="./img/SAP_WEB_IDE.PNG" alt="create device" width="80%">

Please talke 5 minutes and familarize with the SAP Web IDE.
Afterwards, please open the preferences by clicking on the following symbol on the left naviagtion panel.
Verify that the IoT Application Enablement Feature is enabled:

<img src="./img/IOT_AE_FEATURE.PNG" alt="create device" width="80%">

#### Create a new Projekt

After we´ve successfully checked the prerequisite we can now create an new project.
Pleas use "*File* -> *New* -> *Project from Template*":

<img src="./img/NEW_PROJ.PNG" alt="create device" width="80%">

Select IoT Application:

<img src="./img/IOT_APP.PNG" alt="create device" width="80%">

Provide now the "Basic Infomation":

<img src="./img/IOT_AE_BASIC_INFO.PNG" alt="create device" width="60%">

Select the following "OData" Service:

<img src="./img/IOT_AE_SERVICE.PNG" alt="create device" width="60%">

Search the "Property Set":

<img src="./img/IOT_AE_PS_SEARCH.PNG" alt="create device" width="60%">

And all entities and choose next:

<img src="./img/IOT_AE_PS.PNG" alt="create device" width="60%">

In the next screen u can see the pages which are genearted:

<img src="./img/IOT_AE_PAGES.PNG" alt="create device" width="80%">

In the upcomming screens u can maintain each page settings in detail.

Finally u can finish the "Wizard", afterwards u can find the created project in your workspace:

<img src="./img/IOT_AE_PROJECT.PNG" alt="create device" width="50%">

#### Start the application via SAP Web IDE

To verify your application, u can now start easiliy the application by selecting the corresponding folder which is here "iot" and press the "launch" button:

<img src="./img/IOT_AE_APP_LAUNCH.PNG" alt="create device" width="50%">

**Important: Sometimes you need to allow popups from SAP Web IDE, please make sure to allow this**

If u start this app again, you should now see our successfully SAPUI5 app:

<img src="./img/IOT_AE_APP_MAP_01.PNG" alt="create device" width="50%">

But what´s that, if u select your thing you get this popup:

<img src="./img/IOT_AE_APP_MAP_02.PNG" alt="create device" width="50%">

This depends on the fact that we do not has specified an location for our thing.

To do this please go back to the [Thing Modeler](https://sycor-cf-subaccount.iot-sap.cfapps.eu10.hana.ondemand.com/launchpage/index.html#Thing-model&/packages/iotae.sycor.syc.azubi.train/thingtypes/)

Selsct your Thing and provide the Latitude and Longtitude of your device:

Tip u can use "Google Maps" or iam using this tool: https://www.gps-coordinates.net/

<img src="./img/LOCATION.PNG" alt="create device" width="70%">

Save your changes and jump back to the application.

Refresh the application and whooooot u can now find your device on the map:

<img src="./img/MAP_FINAL.PNG" alt="create device" width="70%">

And by selcting the marker you can switch over e.g. the "Analysis Page" to display more data:

<img src="./img/DATA.PNG" alt="create device" width="70%">

Congratulations! you are successfuly finished the third excercise !!!

In the fina (optional) excercise we try to visualize our iot data on our mobile device.

Start here with [Exercise4](../exercise4/README.md)








