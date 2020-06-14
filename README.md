# Codalive-SolutionName_SCDFXIBM

# Short description
Our team members are Foon Si Han, Agnes Woo Jie Lyn, Lai Jing Ying Claudia.
Codalive exists because of our common desire to learn something new and exercise our creativity this Covid holiday. 
Our team name is inspired from 'code' and 'alive', which represents our hope that coding technology can help save lives. 
Together, we have learnt to recognise new challenges and trends towards life saving. 
We have also renewed our admiration and respect towards Front Liners, the heroes of SCDF.  
THANK YOU VERY MUCH FOR YOUR WORK! 

# What's the problem? 
Firefighters are expected to perform their duties in high heat conditions. They face physical and mental challenges during training and operations. 

Problem statement 2: Climate change

"Climate change is inevitable, with the projected increase in temperatures leading to phenomena such as the Urban Heat Island effect. This leads to an environment and climate where it is increasingly physically challenging for First Responders to train and operate to maximum efficiency and performance. How might SCDF leverage wearables or other technologies to provide relief or enhancement in harsh operating conditions and maximise the safety, health and performance of First Responders during training and operations?"

# How can technology help?
We gather heart rate and body temperature data from firefighters using sensors. We can make sense of such data via machine learning, to detect if an officer is overworked or in danger of heat stroke. Moreover, such data may complement optimising training effectiveness. The aim is to use data acquisition and analysis as an additional safeguard on the wellbeing of our heroes. 

# The idea
We use lightweight, low cost sensors as attachment to the firefighter's jacket. They are to detect the firefighter's heart rate and body temperature. During training and operations, data acquired may be analysed real time to alert him/ her and the commanding officer(s) if he/ she is overworked or in danger of heat stroke. Moreover, such data can be kept in the user's own profile records on a web app for self evaluation. 

Additionally, during operations, a portable fan may be attached to a slot in the firefighter's jacket to help fight the heat.  

# Pitch Video

# The architecture 
<img width="960" alt ="2020-06-13" src="https://github.com/sihan00/Codalive-SolutionName_SCDFXIBM/blob/master/Architecture_Design.png">

1. Sensors are linked to a user’s account. 
2. Sensors send data via Bluetooth/WiFi/Lora to Node-RED.
3. IBM DB2 stores acquired data. 
4. We retrieve an instance of Data Asset to IBM Machine Learning model for analysis of health or safety risks. 
5. Processed information is sent over to the user’s account, an alert is issued to commanding officer if any threat is detected.
6. User may access logged data for self evaluation.  


d) A hyperlink to your detailed solution* (Long description of your solution)

# Project Roadmap/ Proposed timeline
<img width="960" alt ="2020-06-13" src="https://github.com/sihan00/Codalive-SolutionName_SCDFXIBM/blob/master/proj%20roadmap.PNG">

f) Getting started* (Step-by-step instructions to install the required software and how to run a demo of your solution)

g) Running the tests (Explanation and breakdown on how to run tests for the proposed solution)

h) Live demo (Link to an actual working demo/website)


*Items marked with an asterisk are compulsory

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
npm install node-red-contrib-db2 node-red-contrib-ttn
```
Configure and connect the TTN uplink node to the Db2 node to enter data into the Db2 database


## On IBM Cloud
Go to your catalogue and create an instance of Watson Studios, Watson Machine Learning, Db2 if they have not been created. 

1. Create a new project on Watson Studio 
2. Create a Db2 database and new credentials for it. Record it
3. At the Watson Studio project, create a connection by add to project and select Db2
4. Configure the connection using the credentials recorded earlier
5. Go back to the Db2 console and run an SQL and choose appropriate Schema to configure the data


# Build With
- The Things Network
- Node-RED
- IBM DB2
- IBM Machine Learning
- REACT WEB APP/IOS/Andriod 

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
