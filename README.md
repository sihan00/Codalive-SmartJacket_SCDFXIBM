# Codalive-SmartJacket_SCDFXIBM

# Short description
Our team members are Foon Si Han, Agnes Woo Jie Lyn, Lai Jing Ying Claudia.
Codalive exists because of our common desire to learn something new and exercise our creativity and be part of something greater than ourselves to contribute to the community this Covid season. 
Our team name is inspired from 'code' and 'alive', which is symbolic of our hope and dream that engineers can not only design the future but also use the power of coding to save lives. 
Together, we appreciate how much we can learn about the different technologies available to recognise new challenges and trends towards doing what we can to put others first and to protect our community during crisis. 
Through researching for the project and creating new innovations to contribute to the process of value adding towards the solutions available for the problem statement, we learnt so much more about the sacrifices and contributions of those working to support the front lines especially during crisis such as the covid-19. 
With this newfound respect and appreciations towards our frontliners, it gives us even more honour and privilege to be able to be part of this opportunity to contribute our ideas and play a part in this process of saving lives, no matter how small it may be.  
THANK YOU VERY MUCH FOR YOUR WORK! 

# What's the problem? 
Firefighters are expected to perform their duties in high heat conditions. They face physical and mental challenges during training and operations. 

Problem statement 2: Climate change

"Climate change is inevitable, with the projected increase in temperatures leading to phenomena such as the Urban Heat Island effect. This leads to an environment and climate where it is increasingly physically challenging for First Responders to train and operate to maximum efficiency and performance. How might SCDF leverage wearables or other technologies to provide relief or enhancement in harsh operating conditions and maximise the safety, health and performance of First Responders during training and operations?"

# How can technology help?
We gather heart rate and body temperature data from firefighters using sensors. We can make sense of such data via machine learning, to detect if an officer is overworked or in danger of heat stroke. Moreover, such data may complement optimising training effectiveness. The aim is to use data acquisition and analysis as an additional safeguard on the wellbeing of our heroes. 

# The idea - SmartJacket
We use lightweight, low cost sensors as attachment to the firefighter's jacket. They are to detect the firefighter's heart rate and body temperature. During training and operations, data acquired may be analysed real time to alert him/ her and the commanding officer(s) if he/ she is overworked or in danger of heat stroke. Moreover, such data can be kept in the user's own profile records on a web app for self evaluation. 

Additionally, during operations, a portable fan may be attached to a slot in the firefighter's jacket to help fight the heat. 

# Pitch Video

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/P2LJPxlXN7I/0.jpg)](https://www.youtube.com/watch?v=P2LJPxlXN7I)

# The architecture 
<img width="960" alt ="2020-06-13" src="https://github.com/sihan00/Codalive-SolutionName_SCDFXIBM/blob/master/Architecture_Design.png">

1. Sensors are linked to a user’s account. 
2. Sensors send data via Bluetooth/WiFi/Lora to Node-RED.
3. IBM DB2 stores acquired data. 
4. We retrieve an instance of Data Asset to IBM Machine Learning model for analysis of health or safety risks. 
5. Processed information is sent over to the user’s account, an alert is issued to commanding officer if any threat is detected.
6. User may access logged data for self evaluation.  

# Project Roadmap/ Proposed timeline
<img width="960" alt ="2020-06-13" src="https://github.com/sihan00/Codalive-SolutionName_SCDFXIBM/blob/master/proj%20roadmap.PNG">


# Getting Started
## Prerequisites
1. IBM Cloud account
2. Sensor and microcontroller of choice
3. The Thing Network account
4. Configured TTN gateway
5. node-RED running locally or on IBM cloud - https://nodered.org/docs/getting-started/ibmcloud

## On The Things Network
After creating your account, enter the console and add an application. Fill in the necessary information and register your IoT device.

## On Node-RED
```
npm install node-red-contrib-db2-fixed node-red-contrib-ttn
```
Configure and connect the TTN uplink node to the Db2 node to enter data into the Db2 database

<img width="960" alt ="2020-06-13" src="https://github.com/sihan00/Codalive-SolutionName_SCDFXIBM/blob/master/Node-RED_connection.png">

## On IBM Cloud
Go to your catalogue and create an instance of Watson Studios, Watson Machine Learning, Db2 if they have not been created. 

1) Create a new project on Watson Studio 
2) Create a Db2 database and new credentials for it. Record the credentials down
3) At the Watson Studio project, create a connection by *add to project* and select Db2
4) Configure the connection using the credentials recorded earlier
5) Go back to the Db2 console and run an SQL and choose appropriate Schema to configure the data
6) Return to Watson Studios project click *add to project*a and select *Connected assets*
7) Choose the configured data from step 5 as the the connection source and click create to create a data asset
8) Click the assets tab in the the Watson studio project and click *New Watson Machine Learning Model" 
9) Create a new model and choose the data asset created the data asset from step 7
10) Save the best performance after the Machine Learning training and evaluation is done
11) Configure the setting under the evaluation tab to add feedback data so that machine learning would evaluate again with new data
12) In the *Depoloyments* tab, click *Add Deployment*, choose *Web service* and save it
13) The Machine Learning Model can be used on under the *Implementation* tab


# Build With
- The Things Network
- Node-RED
- IBM DB2
- IBM Machine Learning
- REACT WEB APP/IOS/Andriod 

## Links

1) node-red db2 - https://flows.nodered.org/node/node-red-contrib-db2-fixed
2) node-red ttn - https://flows.nodered.org/node/node-red-contrib-ttn
3) IBM Watson Studio documentation - https://dataplatform.cloud.ibm.com/docs/content/wsj/getting-started/welcome-main.html
4) watson-continuous-learning-on-db2 - https://github.com/IBM/watson-continuous-learning-on-db2

# Resources available

Challenge resources:  
1) GitHub
2) IBM Cloud 
3) challenge guides - https://iraangeles-ibm.github.io/SCDF-INNOVATION-CHALLENGE/
4) challenge website - https://www.scdf.gov.sg/scdf_innovation_challenge/resources

Idea inspiration: 
1) research paper - https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5796472/
2) research paper - https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6308959/
3) fan jacket - https://qz.com/quartzy/1674873/sonys-new-reon-pocket-is-an-in-shirt-air-conditioner/
