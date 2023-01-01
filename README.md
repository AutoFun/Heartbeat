# An IoT-based Smart Heartbeat Monitoring System
---
This thesis project proposed a wireless heartbeat monitoring system based on the modern IoT
techniques. The system hardware consists of Arduino and its Wi-Fi shield which collect
heartbeat measurements from the heartbeat sensor to the web application via selected
Wi-Fi network. A cloud database was designed and developed to store the incoming
data for data processing. The system is equipped with a mobile application with a
friendly design which allows the user to interact with the system in a smart way.

---
## Proposed system achievements

The proposed system takes advantage of the Arduino Wi-Fi shield which make the
hardware act as a single web server. And the source codes of the web application are
uploaded to an independent folder of Arduino board. The system web application can be
queried wirelessly by a specific URL with a Wi-Fi connection.

This system take advantage of the cloud database developed and maintained by Mongo
Cloud. Compared with the projects which store the data locally or using traditional
database, this system has a high expectancy. Cloud database is suitable for various IoT
frameworks and AI tools. In the future, it can also update with AIoT frameworks.

Similar to many IoT healthcare system projects, the proposed system also has
application to support the services and provide functions. This proposed system has the
web server embedded on the hardware and the function are smarter than a lot of
traditional projects. One feature on the data presentation is the echart was used to add
data visualization features for this project. The data was output as different charts or
diagram to help user to analyse the heartbeat results.

## Tech Stack:
Android app Dev & Ops with Java  
MongoDB Cloud  
Arduino Programming   
Data visualization with Aparche Echart  

## Features：
Self-developed Android Application  
Real-time display  
Data Visualization  
IoT Cloud database
AIOT extension

## Hardware:
Arduino-Yun WIFI-Shield  
Arduino UNO  
MAX30100 sensor  
SD card

## Prototype:

### Mobile application workflow diagram
Start the system mobile application by clicking the icon. In the login page, it requires
the username and password if the account is existed, otherwise the user should register a
new account. Enter the system, there is Home Page which presents the general
information of the system. In many IoT heartbeat monitoring projects, it is important to
remind the user about measurements or any updates about the application. This is
achieved by the Notification layout which is designed using a scroll down view. The
software can get the information of hardware in the Hardware Page, the connection
state, and database record. Hardware state information includes the sensor state,
microcontroller state, hardware battery. The Record Page presents the information about
the detailed record which is obtained from the system database. It can provide the
specific information with different requirements. The Account Page includes
information about the settings, the account information, and the user location.
![image](https://user-images.githubusercontent.com/42330996/210161437-3de5be7c-e0b8-44ba-a54c-2ab6f46a1a1e.png)


## Demo:

### MongoDB Cloud Cluster configuration
![image](https://user-images.githubusercontent.com/42330996/210161380-eab02565-287c-4ab0-8cbd-3b3190f17b3d.png)

### Demo database for data querying purpose
![image](https://user-images.githubusercontent.com/42330996/210161396-72df85fc-8f1a-4683-82da-c41cc352212e.png)

### Application Prototype using Adobe XD
![image](https://user-images.githubusercontent.com/42330996/210161414-785319ba-d170-49b9-acd6-75f755da691f.png)
---
![image](https://user-images.githubusercontent.com/42330996/210161418-d19e80f4-c413-4790-bd1a-514952731bb4.png)
---
![image](https://user-images.githubusercontent.com/42330996/210161428-af1f834f-48fb-49f6-a3d9-b94b555151c8.png)


## Reference:
