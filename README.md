# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/f7eed4bb-a22b-4de0-a57f-f999ed80b74a)


Step 3: A new window will appear. Select “Simple Root Resource” and click Next.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/904f947c-33ae-4307-ab6b-bd8a965c49f0)


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/7230a274-a2f8-4344-b28d-3398eddf524e)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.

Step 6: Alter getHtml() method as shown below.

Step 7: Save your project, clean and build it. Deploy your project.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/c3d45159-2c11-4eec-ba93-ed9815fb9cc5)


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.

Step 2: Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/07a957db-f48a-4fcd-b179-438095c5eaae)


Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 

Step 4: Carefully select your RESTful resource (web service) and click OK.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/5a4769dc-6812-4158-8265-bc6a2fa9a554)
 

Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/198b1abc-3a39-4d68-86b3-047cf9575b56)


Step 6: An editing tab will open. Alter getHtml() method with the following.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/6a52dffb-3a5b-43f7-807e-afdd201f08a3)



Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/27352822-bb47-46c8-83d5-9676e68c225d)



Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/197db1fb-d16b-4867-870b-369cae6eef46)



Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.

Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/15f46016-b6fe-4311-83d3-b7a54edb88df)


Step 11: Save the project and build it.


Step 12: Run the JSP file and you should see the output in a new browser window.

![image](https://github.com/Kaviarasu510/Ex-04_RESTful_Web_Services/assets/119392695/28fa573c-d1f0-491a-88cf-b04c2d08dff2)




Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2

Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";

Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
