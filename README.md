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

### System mobile application folder tree
```
Heartbeat/	  
├─ app/	  
│  ├─ manifests/	  
│  ├─ java/	  
│  │  ├─ com.example.heartbeat/	  
│  │  │  ├─ fragment/	The folder of frontend page connection  
│  │  │  │  ├─ fragmentHome.java	Java class for the Home fragment  
│  │  │  │  ├─ fragmentHardware.java	Java class for the Hardware fragment  
│  │  │  │  ├─ fragmentData.java	Java class for the Data fragment  
│  │  │  │  ├─ fragmentRecord.java	Java class for the Record fragment  
│  │  │  ├─ sensor/	  
│  │  │  │  ├─ sensorData.java	  
│  │  │  ├─ setting/	  
│  │  │  │  ├─ setting.java	  
│  │  │  │  ├─ settingsAdapter.java	  
│  │  │  ├─ showData/	  
│  │  │  │  ├─ getHardwareState.java	Get data from database and show them in the hardware page  
│  │  │  │  ├─ getHeartbeatData.java	  
│  │  │  │  ├─ getRecord.java	  
│  │  │  ├─ user/	
│  │  │  │  ├─ RegisterActivity.java	The register logic  
│  │  │  │  ├─ user.java	  
│  │  │  │  ├─ LoginActivity.java	The login logic  
│  │  │  ├─ home.java	Home page backend code   
│  │  │  ├─ MyFragment.java	Fragment adaptor  
│  ├─ res/	  
│  │  ├─ drawable/	  
│  │  │  ├─ icon.xml	  
│  │  ├─ layout/	  
│  │  │  ├─ activity.xml	The frontend layout  
│  │  ├─ mipmap/	  
│  │  │  ├─ icon.png	Icon image  
│  │  ├─ values/	  
│  │  │  ├─ styles.xml	The colour, font,   
│  ├─ assets/	  
│  │  ├─ echart.js	Contains the project echart JavaScript  
├─ Gradle Scripts/	   
│  ├─ build.gradle	  
```
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
![image](https://user-images.githubusercontent.com/42330996/210161473-cefe6276-ff2f-4288-85c2-1e0366ac87ed.png)


## Reference:
[1] N. Holter, “New Method for Heart Studies”, Annals of Noninvasive Electro
cardiology, vol. 3, no. 4, pp. 381-387, 1998.  
[2] S. Akselrod, D. Gordon, F. Ubel, D. Shannon, A. Berger and R. Cohen,
“Power spectrum analysis of heart rate fluctuation: a quantitative probe of beat-to
beat cardiovascular control”, Science, vol. 213, no. 4504, pp. 220-222, 1981.  
[3] V. Pichot, F. Roche, J. Gaspoz, F. Enjolras, A. Antoniadis, P. Minini, F. Costes
and T. Busso, “Relation between heart rate variability and training load in middle
distance runners”, Medicine & Science in Sports & Exercise, vol. 32, no. 10, pp.
1729-1736, 2000.  
[4] T. Salomi; S. Amar; S. Anurag; B. Vishal, “Sensing heartbeat and body temperature
digitally using Arduino,” in IEEE Intern. Conf. on Signal Processing, Communication,
Power and Embedded System (SCOPES), Paralakhemundi, India, Jun. 2017.  
[5] Z. Zhilin, “Photoplethysmography-Based Heart Rate Monitoring in Physical
Activities via Joint Sparse Spectrum Reconstruction,” IEEE Trans. Biomedical
Engineering, vol. 62, no. 8, pp. 1902-1910, Feb. 2015.  
[6] F. Mohamed, B. Mounir, and B. Mouldi, “Microcontroller Based Heart Rate
Monitor,” The International Arab Journal of Information Technology (IAJIT), Vol. 5, No.
4, Oct. 2008.  
[7] T. Arulananth and B. Shilpa, "Fingertip based heartbeat monitoring system
using embedded systems", in Intern. Conf. on Electronics, Communication and
Aerospace Technology, 2017.  
[8] Y. Kurzweil-Segev et al., “Remote monitoring of phasic heart rate changes
from the palm,” IEEE Trans. THz Sci. Technol., vol. 4, no. 5, pp. 618–623, Sep.
2014.  
[9] K. Junhyung et al., “Capacitive Heart-Rate Sensing on Touch Screen Panel with
Laterally Interspaced Electrodes,” in Sensors, Jul. 2020.  
[10] T. S. Arulananth, B. Shilpa, A. Shadi, “Fingertip based heartbeat monitoring
system using embedded systems,” in Intern. Conf. on Electronics, Communication and
Aerospace Technology (ICECA), Coimbatore, India, Dec. 2017.  
[11] I.V. Mikhelson, S. Bakhtiari, T.W. Elmer, and A.V. Sahakian, “ Remote sensing of
heart rate and patterns of respiration on a stationary subject using 94-GHz
millimeter-wave interferometry ,” IEEE Trans. Biomedical Engineering, vol. 58, no. 6,
pp. 1671-1677, 2011.  
[12] A. Sani, “An IoT-Based Smart Framework for a Human Heartbeat Rate
Monitoring and Control System,” in IEEE Intern. Conf. on Sensors and Applications,
Nov. 2019.  
[13] R. Aritra, R. Hena, “Secured Pulse Rate Monitoring System using IoT and Cud,”
in IEEE Intern. Conf. on Emerging Frontiers in Electrical and Electronic Technologies
(ICEFEET), Paralakhemundi, Patna, India, Sep. 2020.  
[14] Akanksha, Eisha, “Framework for propagating stress control message using
heartbeat based IoT remote monitoring analytics,” International journal of
electrical and computer engineering (IJECE), Vol. 10, No.5, pp.4615-4622, Oct. 2020.
[15] Z. Zhilin, “Photoplethysmography-Based Heart Rate Monitoring in Physical
Activities via Joint Sparse Spectrum Reconstruction,” IEEE Trans. Biomedical
Engineering, vol. 62, no. 8, pp. 1902-1910, Feb. 2015.  
[16] A. Kahtan, T. Saed, I. Salah, A. Shadi, “Smart real-time healthcare monitoring and
tracking system using GSM/GPS technologies,” in 3rd MEC Intern. Conf. on Big Data
and Smart City (ICBDSC), Muscat, Oman, Apr. 2016.  
[17] Y. Geng et al., “A Health-IoT Platform Based on the Integration of Intelligent
Packaging, Unobtrusive Bio-Sensor, and Intelligent Medicine Box,” IEEE Trans.
Industrial Informatics, vol. 10, no. 4, pp. 2180-2191, 2014.  
[18] S. Jayanth, M. Poorvi, R Shreyas, B. Padmaja, M. Sunil, “Wearable Device to
Measure Heartbeat using IoT,” in Intern. Conf. on Inventive Systems and Control
(ICISC), Coimbatore, India, Oct. 2017.  
[19] G. Pankaj, “Selecting the right IoT cloud platform,” in Intern. Conf. on Internet
of Things and Applications (IOTA), Pune, India, Jan. 2016.  
[20] Z. Haikun, “Design anImplemention of Poultry Farming Information
Management System Based on Cloud Database,” Animals, Basel, Vol. 11, Oct. 2021.
[21] T. Asoke, H. Roland, “AIoT: AI meets IoT and Web in Smart Healthcare,” in
ACM Web Science Conference, Applications and Services, New York, NY, United
States Jun. 2021.  
[22] L. Yu-Jin et al., “An AIoT Wearable ECG Patch with Decision Tree for Arrhythmia
Analysis,” in IEEE Intern. Conf. on Biomedical Circuits and Systems Conference
(BioCAS), Nara, Japan, Oct. 2019.  
[23] P. Shekhar, “Machine Learning and IoT for Prediction and Detection of Stress,”
in Intern. Conf. on Computational Science and Its Applications (ICCSA), Trieste, Italy,
Jul. 2017.  
[24] Z. Zixuan, H. Tianyiyi, Z. Minglu, S. Qiongfeng, L. Chengkuo, “Smart Triboelectric
Socks for Enabling Artificial Intelligence of Things (AIoT) Based Smart Home and
Healthcare,” in IEEE Intern. Conf. on Micro Electro Mechanical Systems (MEMS),
Vancouver, BC, Canada, Jan. 2020.  
[25] N. Mzomuhle, “Chllenges in mobile bio-sensor based mHealth development,”
in Intern. Conf. on e-Health Networking, Applications and Services, Columbia, MO,
USA, Sep. 2011.  
[26] T. Salomi; S. Amar; S. Anurag; B. Vishal, “Sensing heartbeat and body
temperature digitally using Arduino,” in IEEE Intern. Conf. on Signal Processing,
Communication, Power and Embedded System (SCOPES), Paralakhemundi, India, Jun.
2017.  
[27] “Getting Started with Arduino UNO” [online] arduino.cc/en/Guide/ArduinoUno
Available at: https://www.arduino.cc/en/Guide/ArduinoUno [Accessed 3 May. 2021].
[28] S. S. Thomas, A. Saraswat, A. Shashwat, and V. Bharti, “Sensing heart beat and
body temperature digitally using Arduino,” in 2016 International Conference on
Signal Processing, Communication, Power and Embedded System, pp. 1721–1724,
2016,.  
[29] H. Fukushima, H. Kawanaka, M.S.Bhuiyan, K. Oguri, “Estimating heart rate using
wrist-type photoplethysmography and acceleration sensor while running”, Annual
International Conference of the IEEE, pp. 2901–2904, 2012.  
[30] “Interfacing MAX30100 Pulse Oximeter Sensor with Arduino” [online]
mongodb.com/cloud/atlas Available at: https:// how2electronics.com/interfacing-
max30100-pulse-oximeter-sensor-arduino/ [Accessed 11 May. 2021].  
[31] J. Wan, Y. Zou, Y. Li, and J. Wang, “Reflective type blood oxygen saturation
detection system based on MAX30100,” 2017 Int. Conf. Secur. Pattern Anal. Cybern.
SPAC 2017, vol. 2018-Janua, no. 4, pp. 615–619, 2018.  
[32] Z. Zhang, “Photoplethysmography-Based Heart Rate Monitoring in Physical
Activities via Joint Sparse Spectrum Reconstruction,” IEEE Trans Biomed Eng,
vol.62, no. 8, pp. 1902-1910, 2015 .  
[33] “Global multi-cloud database” [online] mongodb.com/cloud/atlas Available at:
https://www.mongodb.com/cloud/atlas [Accessed 15 May. 2021].  
[34] “The database for modern applications” [online] mongodb.com Available at:
https://www.mongodb.com/ [Accessed 20 May. 2021].  
[35] “The database for modern applications” [online] mongodb.com Available
Available at: https://www.mongodb.com/ [Accessed 15 May. 2021].  
[36] “MongoDB Compass-The easiest way to explore and manipulate your MongoDB
data” [online] mongodb.com/products/compass Available at:
https://www.mongodb.com/products/compass [Accessed 16 May. 2021].  
