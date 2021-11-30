# Challenge 2 - Function App

Azure functions is a serverless concept of cloud native design that allows a piece of code to be deployed and executed without any need of server infrastructure, web server, or any configurations. Azure functions can be written in multiple languages such as Powershell, C#, Java, JavaScript, TypeScript, and Python.

An Azure Function is ideal for running code that gets triggered by a certain event.
- HTTP trigger (a GET, POST, PUT, ... call is being made towards the function url)
- Timer trigger (at a certain moment in time the function will run)
- ...

For example, you could use an Azure Function for the following use cases:
- At 10:00 AM every day, send an email to a list of users with a report of the last 24 hours of their usage
- When somebody uploads a CSV to a storage account in Azure, transform that CSV into a JSON object and store it in a different blob storage
- I want a simple HTTP Get endpoint that fetches a JSON object from a storage acocunt and returns the contents of that file (this is a very simple API)


## Instructions for Jill

Hey Jill,

I created an Azure Function which will return the necessary proof of my supremacy.

It is simple. The function will call another endpoint which will return the necessary data.
So head over to `run.ps1` and fill in the missing URL which I'll send **via a different channel**.
The other endpoint is expecting it to be called with Post request and the following JSON body:
```json
{
    "sendFakeDonaldData": true
}
```


I tried to run it but looks like there are also a couple of bugs in the code... At least it is not returning the correct value.
So yeah, it is nearly complete but you will have finish it up. 


To deploy the function to Azure, you best use the VSCode extension called Azure Functions.
Then use the command pallet (ctrl+shift+p) to login to azure. (Azure: Sign in)\
This will allow you to deploy the function to Azure by right clicking on the challenge-2 folder and selecting `Deploy to Function App...`\
![deploy](https://i.imgur.com/S7PUEdR.png))\
I already setup a function app to which you must deploy the function. You cannot use any other or it will not work.

After you deployed it, it will have an URL which you can use to test it. Find this url in VSCode or in the Azure portal.

Good luck!
