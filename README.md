We first start by setting up the docker environment
![image](https://github.com/user-attachments/assets/23d07d3e-42ca-4b46-aba0-224f7ea319f6)
![image](https://github.com/user-attachments/assets/1b186676-c632-4aeb-ad36-718e86028af5)

[image](https://github.com/user-attachments/assets/f41b7851-215e-4421-b1e9-62ed2ee9a4e6)
Next, the data from the server is sent to the local host by using docker, and from there, we start exploiting the data. This exploitation is done by nip. which allows us to map any ip address. After the hosting is done, we generate the payloads from the source code and push them to the local host.
![image](https://github.com/user-attachments/assets/65924498-a73d-4571-9346-773df20b53c2)
![image](https://github.com/user-attachments/assets/d215fb3d-a866-4c65-984d-d9b3207a0135)
Next we made sure that using the docker logs command , payload is pushed into the server.
![image](https://github.com/user-attachments/assets/26b27148-6420-4e3d-8032-3d2cdb314953)
The curl flag is generated using the local host flag curl command it is not able to push into the server, so we switched and pushed into the Redis payload
![image](https://github.com/user-attachments/assets/913d2051-dedf-4e15-ae71-ed3a7e857e7c)
![image](https://github.com/user-attachments/assets/fc0ef9f5-5151-4895-b4f2-0c80162b3c55)

CODE 
![image](https://github.com/user-attachments/assets/bb995fc6-29f3-44c9-b74b-a7575dda8114)
This script simulates a web challenge scenario inspired by HackTheBox write-ups. It starts by mapping the IP address and port using nip.io, initializes Redis with necessary keys, and injects a payload that commands the server to download a webshell. After sending the payloads, it tries to retrieve the flag. If successful, the server's behavior indicates tampering, which is detected by the script.
