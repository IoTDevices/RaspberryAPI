<h3>Raspberry API - what is it?</h3>

An IoT Device API Server, utilising oAuth2, OWIN, and MVC, over HTTP

<h3>How do I install it</h3>

Either pull the code - or use the Visual Studio Extension at https://github.com/IoTDevices/RaspberryAPI/tree/master/VSIX%20Installer

Note: The advantage of using the Visual Studio Extension is that when you go "File / New Project / (etc)" you can choose your own namespace.

<H3>How do I configure it?</H3>

You will first have to add your SQL Server connection details to Web.config, as per the following:

```
  <connectionStrings>
    <add name="AuthContext" connectionString="Server={put your details here}" providerName="System.Data.SqlClient" />
  </connectionStrings>
```

Then, just build and deploy the server!

The first time you that you Register a user, all of the tables will be automatically generated in the SQL Server database.

Then, you will have to add a row to the clients table, to identify each application that your users can use.

Once you have a minimum of just one row added to that table, you can start testing your server over Http using a client like Chrome's 'Postman' extension.

It's just that easy!

For full details, please read our wiki here!

https://github.com/IoTDevices/RaspberryAPI/wiki

We will have progressively more written here about the Raspberry API Server, here in the next few weeks!

