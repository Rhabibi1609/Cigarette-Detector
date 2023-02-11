# Cigarette Detector WebApp (a project for FRT internship)

It is a WebApp that uses html,css,js,python,flask and services of azure(custom vision and app service). The custom vision is trained on images of cigarette and detects it as an object. (please note that it is just a demonstration).

> Demo Video Link: https://youtu.be/iTfyIPZ1V-M
> Live Project Link: https://smokerdetecting.azurewebsites.net/



# To Run:
> * Open https://smokerdetecting.azurewebsites.net/
> * click on upload and upload a picture.
> * press on predict.

PIP Requirements:
* azure-cognitiveservices-vision-customvision==3.1.0
* Flask==2.0.2
* matplotlib==3.5.1
* msrest==0.6.21
* numpy==1.22.1
* Pillow==9.1.1
* python-dotenv==0.20.0


# Steps for Custom Vision: 
> Open Azure Portal and Sign in with your account.
> For CUSTOM VISION:
> 1. Create a custom vision resource.
> 2. Go to Custom vision portal
> 3. Create a project.
> 4. Select Object Detection and configure it to a resource group by selecting a resource group.
> 5. Upload some (min 20) images and label it.
> 6. Use the prediction key to predict from a program.

![download](https://user-images.githubusercontent.com/77888595/218259720-335c6e5d-1991-466c-a8e4-4c70e248f5b0.png)


# Steps for App Service: 
> Open Azure Portal and Sign in with your account.
> 1.Create an app service (web app) resource.
> 2.In configuration tab, select resource group and give unique name for both resource group and web-app.
> 3.Select Runtime Stack as Python 3.10.
> 4.Go to Deployment center and choose a method to upload your source code (I used github (github actions)).
> 5. Wait for deployment.
> 6. Find Your website live on https://.azurewebsites.net/

![image](https://user-images.githubusercontent.com/77888595/218259731-1653cfe6-0570-4776-8c7b-1afb0f521c64.png)
