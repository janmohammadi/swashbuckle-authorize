# Swagger Authorize
Enables authentication and authorization for Swagger (Swashbuckle) in WebApi projects.

What it looks like:
![How it works](https://cdn.pbrd.co/images/Hg2NkLw.gif)

How to use:

1- Download and copy `SwaggerAuthorization.js` file in to Scripts folder.

2- Right click on the `SwaggerAuthorization.js` file > Properties > Build Action and select Embeded Resource.

3- Add the line below to the App_Start\SwaggerConfig.cs file, in EnableSwaggerUi section: 
```cs
c.InjectJavaScript(thisAssembly, "YOUR_PROJECT_NAMESPACE.Scripts.SwaggerAuthorization.js");
```
