# Project Title : OAuth module enhancements and SMART apps support

##### **Primary Mentor  :** Sanatt Abrol
##### **Backup Mentor   :** Harsha Kumara
##### **Student         :** Prabodh Kotasthane
##### **Project wiki    :** []()

#### Major Objectives : 
* **Registration of SMART clients/application RESTfully**
* **Integration of SMART's EHR Launch Flow**
* **Functionality of Scopes and Launch Context**

#### Extra Crefit : 
* **Open Web Application supporting SMART**

#### Project Overview :
##### Registration of SMART clients/application RESTfully
In order to be able to run SMART apps from the EHR, i.e. OpenMRS, user is first needed to register the respective SMART application/client. A SMART client is no different than a normal OAuth client except that it must have a Launch Url which is the SMART app launch url to which the browser would redirect when the user attempts to run SMART apps. This objective involved adding the required new tables for the SMART application, also adding the respective DAOs and Services. The functionality to register and modify a SMART application  was added by modifying the existing REST controllers to manage OAuth Clients.

##### Integration of SMART's EHR Launch Flow
The EHR launch flow of SMART apps is properly integrated within the module. Now a user may see the list of registered SMART application and is able to run them from within OpenMRS. Whenever the user hits "Run", a random launch value is generated and saved in the database, and passed to the SMART application. The application, at the time of requesting authorization, sends back the launch value which is verified to ensure that the SMART app ran in same session. This objective also involved changing the metadata controller so as it gives the metadata response in proper conformance statement format as the SMART apps require.

##### Functionality of Scopes and Launch Context
##### Source Code and Downloads :
+ *Source Code for OpenMRS OAuth2 Module :* [https://github.com/openmrs/openmrs-module-oauth2/tree/gsoc-18](https://github.com/openmrs/openmrs-module-oauth2/tree/gsoc-18)
+ *Source Code for SMART OWA :* [https://github.com/PKatGITHUB/openmrs-owa-smartowa](https://github.com/PKatGITHUB/openmrs-owa-smartowa)
+ *Download OpenMRS OAuth2 Module 2.0 .omod file :* [https://github.com/PKatGITHUB/GSoC-2018-Final-Evaluations/blob/master/oauth2-2.0.omod](https://github.com/PKatGITHUB/GSoC-2018-Final-Evaluations/blob/master/oauth2-2.0.omod)
+ *Download SMART OWA .zip bundle :* [https://github.com/PKatGITHUB/GSoC-2018-Final-Evaluations/blob/master/smartowa.zip](https://github.com/PKatGITHUB/GSoC-2018-Final-Evaluations/blob/master/smartowa.zip)

##### JIRA Issues I have worked on and respective Pull Requests :
+ **[OA-8](https://issues.openmrs.org/browse/OA-8)** : [https://github.com/openmrs/openmrs-module-oauth2/pull/6](https://github.com/openmrs/openmrs-module-oauth2/pull/6)
+ **[OA-9](https://issues.openmrs.org/browse/OA-9)** : [https://github.com/openmrs/openmrs-module-oauth2/pull/7](https://github.com/openmrs/openmrs-module-oauth2/pull/7)
+ **[OA-10](https://issues.openmrs.org/browse/OA-10)** : [https://github.com/openmrs/openmrs-module-oauth2/pull/8](https://github.com/openmrs/openmrs-module-oauth2/pull/8)
+ **[OA-11](https://issues.openmrs.org/browse/OA-11) and [OA-12](https://issues.openmrs.org/browse/OA-12)** : [https://github.com/openmrs/openmrs-module-oauth2/pull/11](https://github.com/openmrs/openmrs-module-oauth2/pull/11)
+ **[OA-13](https://issues.openmrs.org/browse/OA-13)** : [https://github.com/openmrs/openmrs-module-oauth2/pull/12](https://github.com/openmrs/openmrs-module-oauth2/pull/12)
+ **[OA-14](https://issues.openmrs.org/browse/OA-14)** : [https://github.com/openmrs/openmrs-module-oauth2/pull/13](https://github.com/openmrs/openmrs-module-oauth2/pull/13)
+ **[OA-15](https://issues.openmrs.org/browse/OA-15)** : [https://github.com/openmrs/openmrs-module-oauth2/pull/14](https://github.com/openmrs/openmrs-module-oauth2/pull/14) and [https://github.com/openmrs/openmrs-module-oauth2/pull/15](https://github.com/openmrs/openmrs-module-oauth2/pull/15)
+ **[OA-17](https://issues.openmrs.org/browse/OA-17)** : [https://github.com/openmrs/openmrs-module-oauth2/pull/16](https://github.com/openmrs/openmrs-module-oauth2/pull/16)
+ **[OA-18](https://issues.openmrs.org/browse/OA-18)** : [https://github.com/openmrs/openmrs-module-oauth2/pull/17](https://github.com/openmrs/openmrs-module-oauth2/pull/17)



