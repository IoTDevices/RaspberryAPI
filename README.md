<h3>Raspberry API - what is it?</h3>

An IoT Device API Server, utilising oAuth2, OWIN, and MVC, over HTTP

<h3>How do I install it</h3>

Either pull the code - or use the Visual Studio Extension at https://github.com/IoTDevices/RaspberryAPI/tree/master/VSIX%20Installer

Note: The advantage of using the Visual Studio Extension is that when you go "File / New Project / (etc)" you can choose your own namespace.

<H3>How do I configure it?</H3>

You will have to add your SQL Server connection details to Web.config, as per the following:

```
  <connectionStrings>
    <add name="AuthContext" connectionString="Server={put your details here}" providerName="System.Data.SqlClient" />
  </connectionStrings>
```

The first time you Register a user, all of the tables will be automatically generated in the SQL Server database.

Note: I need to add the instructions on what information to add to the Clients table, and how to test the server using the Chrome 'Postman' extension.

Watch this space!

