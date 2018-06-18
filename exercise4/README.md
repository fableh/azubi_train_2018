
### Excercise 4 - Mobilize your IoT Data with SAP Mobile Cards

#### Enter the SAP Cloud Platform Cockpit

[SAP Cloud Platform Cockpit](https://account.hana.ondemand.com/cockpit#)

Enter first the SAP Cloud Platform Global Account "**SAP CP**":

<img src="./img/SCP_Cockpit.PNG" width="60%">

Now enter the Sub Account "**Development**":

<img src="./img/SCP_COCKPIT_SUB.PNG" width="60%">

You should now see a lot of different menu items, feel free to discover the different options:

<img src="./img/SCP_MAIN.PNG" width="60%">


#### Start SAP Mobile Services

From the left menu please switch over to the "Sewrvices":

<img src="./img/SCP_SERVICES.PNG" width="60%">

You cann now search for the different services, scroll down or easier specify the category.
Based on the fact that we want to develop a mobile application we can easily use the dropdown and select "**mobile services**":

<img src="./img/SCP_SERVICES_CATEGORIES.PNG" width="40%">

Enter now the right tile "**Development & Operations, std**":

<img src="./img/SCP_ENTER_MOBILE_TILE.PNG" width="60%">

And finally "**Go to the Service**" by clicking on the link:


<img src="./img/SCP_ENTER_MOB_SERVICE.PNG" width="60%">

#### Discover the "proxy" OData Service for your Thing

Based on the fact, that the data access for SAP Application Enablement works only with OAuth 2.0.
We´ve prerpared an Node JS proxy application which allows u to fetch the data with basic authentification from your thing.

Please use for testing the follwoing credentials:

| User | Password |
| --- | --- |
| foo | bar|

The URL mus be adjusted a bit, the syntax is the follwoing:

https://sap-proxy.cfapps.eu10.hana.ondemand.com/app.svc/measurements?$filter=id eq '**your-thing-id**' and time ge datetime'2018-06-15T00:00:00' and time lt datetime'2018-06-16T00:00:00'&$format=json&$top=3

**Please Adjust the datetime value to a valid period where u sure that the data was send successfully into SAP Application Enablement.**

As result u should now see the following response:

<img src="./img/ODAT_RESP_PRXY.PNG" width="80%">


[SAP Mobile Cards Client for Android](https://play.google.com/store/apps/details?id=com.sap.content2go)


[SAP Mobile Cards Client for iOS](https://itunes.apple.com/us/app/sap-content-to-go/id1168110623?mt=8)

https://sap-proxy.cfapps.eu10.hana.ondemand.com/app.svc/measurements?

$filter=id eq '**your-thing-id**' and time ge datetime'2018-06-15T00:00:00' and time lt datetime'2018-06-16T00:00:00'&$format=json&$top=3
