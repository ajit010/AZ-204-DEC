# AZ-204  24-27 DEC

LAB 1 -- Craete an Azure Function App

    1. Hosting plan -- Consumption

    2. Networking -- enable public access

    3. Create it ..


LAB 2 -- Create a function in portal

    1. Create a Http trigger function in VS Code

    2. Follow the link "https://microsoftlearning.github.io/mslearn-azure-developer/instructions/azure-functions/01-functions-create-                vscode-http.html" for instructions.


Commands :

    1. ssh ajitadmin@<public-ip>

    pswd : <enter> (invisible)

    2.  sudo apt update
    3  sudo apt install apt-transport-https ca-certificates curl software-properties-common
    4  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
    5  echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg]                 https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
    6  sudo apt update
    7  apt-cache policy docker-ce
    8  sudo apt install docker-ce
    9  sudo systemctl status docker
    
More commands :

     11.  docker --version
     12.  docker pull ubuntu
     13   sudo docker pull ubuntu
     14   sudo docker pull ubuntu:22.04
     15   sudo docker images
     16  docker run -dt --name c1 ubuntu
     17  sudo docker run -dt --name c1 ubuntu
     18  clear
     19  sudo docker ps
     20  sudo docker exec -it c1 bash
     21  ls
     22  sudo docker exec -it c1 bash
     23  history
    

       25  docker images
       26  sudo docker images
       27  git clone https://github.com/ajit010/My-Docker-App.git
       28  ls
       29  cd My-Docker-App/
       30  ls
       31  cat Dockerfile
       32  clear
       33  docker build -t myflaskapp .
       34  sudo docker build -t myflaskapp .
       35  clear
       36  docker images
       37  sudo docker images
       38  docker run -dt -p 80:8080 myflaskapp:latest
       39  sudo docker run -dt -p 80:8080 myflaskapp:latest
       40  sudo docker ps
       41  history

 Create an Azure Container Registry and Push Container Image to ACR:
 
       43 sudo docker images
       44  docker tag myflaskapp ajit22.azurecr.io/myflaskapp
       45  sudo docker tag myflaskapp ajit22.azurecr.io/myflaskapp
       46  docker login ajit22.azurecr.io
       47  sudo docker push ajit22.azurecr.io/myflaskapp
       48  history

 Deploy WebApp Using ACR image

       1. Create an azure webapp (publish -- container)

       2. Image - ACR, Aurhentication - Admin Creds

       3. Review n Create.

       4. Finally, you wills see output in Domain URL.

===========================================================================================================================



    


    
