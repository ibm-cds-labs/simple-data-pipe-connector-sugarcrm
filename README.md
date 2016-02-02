# Simple Data Pipe Connector for SugarCRM

##### [Simple Data Pipe](https://developer.ibm.com/clouddataservices/simple-data-pipe/) connector for [SugarCRM](http://www.sugarcrm.com/)

### Pre-requisites

##### General 
The connector is compatible with SugarCRM servers supporting [SugarCRM REST API v4](http://support.sugarcrm.com/Documentation/Sugar_Developer/Sugar_Developer_Guide_7.6/API/Web_Services/API_Versioning/) and OAuth 1.0  (i.e., SugarCRM 6.2.x or greater).

##### Install the SugarCRM connector

Install the connector using [these instructions](https://github.com/ibm-cds-labs/pipes/wiki/Installing-a-Simple-Data-Pipe-Connector) into the Simple Data Pipe.  

##### Enable OAuth support and collect connectivity information

Before the Simple Data Pipe can connect to SugarCRM, complete these steps:

1. Log into SugarCRM.
2. Go into the OAuth page ( __> Admin > OAuth Keys__ ).
3. Click __Create__.
4. Enter a __Consumer Key Name__, __Consumer Key__, and __Consumer Secret__.  

	###### SugarCRM OAuth Keys page:
	![SugarCRM OAuth Keys page] (https://github.com/ibm-cds-labs/pipes.connector.sugarcrm/blob/master/resources/sugarcrmoauthkeys.png)  
5. Click __Save__.

### Using the Sugar CRM Connector 

1. Open the Simple Data Pipe web console.
2. Select __Create A New Pipe__.
3. Select __Sugar CRM__ for the __Type__, provide a unique pipe __Name__ (e.g. my sugarcrm demo pipe) and an optional __Description__.
  ![Create A New Pipe dialog] (https://github.com/ibm-cds-labs/pipes.connector.sugarcrm/blob/master/resources/pipescreatenewpipe.png)
4. In the Connect page, enter the OAuth __Consumer Key__ and __Consumer Secret__.
5. In the Connect page, enter the __Site url__ taken from the `site_url` in SugarCRM's `config.php`.  

	###### Pipes Connect page:
	![Pipes Connect page] (https://github.com/ibm-cds-labs/pipes.connector.sugarcrm/blob/master/resources/pipesconnectpage.png)  

#### License 

Copyright [2015-2016] [IBM Cloud Data Services]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

### Resources

* [SugarCRM 6.x API Versioning] (http://support.sugarcrm.com/02_Documentation/04_Sugar_Developer/Sugar_Developer_Guide_6.5/02_Application_Framework/Web_Services/04_Versioning/)
* [SugarCRM 6.x OAuth] (http://support.sugarcrm.com/02_Documentation/04_Sugar_Developer/Sugar_Developer_Guide_6.5/02_Application_Framework/Authentication/Oauth/)
* [SugarCRM 6.x REST] (http://support.sugarcrm.com/02_Documentation/04_Sugar_Developer/Sugar_Developer_Guide_6.5/02_Application_Framework/Web_Services/01_REST/)
* [SugarCRM v4 REST API] (http://support.sugarcrm.com/02_Documentation/04_Sugar_Developer/Sugar_Developer_Guide_6.5/02_Application_Framework/Web_Services/05_Method_Calls/)
