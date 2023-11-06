# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.


![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/0d6390a8-2187-425a-8687-9adb191a0609)


Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
 
![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/9c8480ec-47d1-4076-8612-afb64f3d00c0)


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/327bbfac-21c8-4ca9-acd4-79084f1286ca)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 

![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/bedcf151-4c41-4527-b4e2-c89215e90682)

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.


![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/17cb3c45-0567-44aa-b40f-6b371f951d8e)



Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
Step 4: Carefully select your RESTful resource (web service) and click OK. 
 

![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/4eac105a-e78a-47ae-adec-f94fbe89511e)


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/a309c248-b16e-480a-945a-024e9fa20ff5)


Step 6: An editing tab will open. Alter getHtml() method with the following.

 ![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/78b5bd87-117a-415f-9f7f-02230c482000)

 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/a77d5654-846a-4951-a8de-c0bcb0ad3aed)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 

 ![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/9142e556-df0c-4e49-bbeb-76782817f614)



Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.


![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/48ce2483-9998-410c-bc77-9db49573790f)

Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.

 ![image](https://github.com/Harishragav123/Ex-04_RESTful_Web_Services/assets/135584731/3b68cdfc-2eef-4a31-9529-d932018ac3c8)

 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
