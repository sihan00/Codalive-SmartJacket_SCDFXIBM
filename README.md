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
<img width="960" alt ="2020-06-13" src="https://github.com/sihan00/Codalive-SolutionName_SCDFXIBM/blob/master/ArchitectureDesign.png">
- Sensors are linked to a user’s account. 
- Sensors send data via Bluetooth/WiFi/Lora to Node-RED.
- IBM DB2 stores acquired data. 
- We retrieve an instance of Data Asset to IBM Machine Learning model for analysis of health or safety risks. 
- Processed information is sent over to the user’s account, an alert is issued to commanding officer if any threat is detected.
- User may access logged data for self evaluation.  


d) A hyperlink to your detailed solution* (Long description of your solution)

# Project Roadmap/ Proposed timeline
<img width="960" alt ="2020-06-13" src="https://github.com/sihan00/Codalive-SolutionName_SCDFXIBM/blob/master/proj%20roadmap.PNG">

f) Getting started* (Step-by-step instructions to install the required software and how to run a demo of your solution)

g) Running the tests (Explanation and breakdown on how to run tests for the proposed solution)

h) Live demo (Link to an actual working demo/website)


*Items marked with an asterisk are compulsory
 
# Build With
- Node-RED
- IBM DB2
- IBM Machine Learning
- REACT WEB APP/IOS/Andriod 

# Resources available

Link: https://iraangeles-ibm.github.io/SCDF-INNOVATION-CHALLENGE/
1) GitHub
2) IBM Cloud 
