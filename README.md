## Demo Application

Basic Todo application with ASP.NET Core 2.1 WEB API as backend. 

Built using Visual Studio for Mac and Visual Studio Code. Container images are created using Docker for Mac. Application was tested against minikube running within a Mac machine. All the below mentioned steps should work everywhere irrespective of Windows/Linux/Mac.

## Prerequisites 

* Visual Studio
* .NET Core SDK 2.1
* Docker for Windows/Docker for Mac

* Create the docker image

    Run the below command to build the docker image
    <pre><code> docker build -t k8s-todo-api:latest . </code></pre>

* Run the API app in a container
  
    Run the below command to run the image in a container
    <pre><code> docker run -p 5000:5000 k8s-todo-api:latest </code></pre>

## Verifaction

* Browse the swagger ui for the api using http://URL:5000/swagger/index.html 