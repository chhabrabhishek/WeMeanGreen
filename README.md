# Smart Collar, Save the Wildlife

## Contents
- [Smart Collar, Save the Wildlife](#submission-or-project-name)
    - [Contents](#contents)
    - [Short description](#short-description)
  - [Demo video](#demo-video)
  - [The Architecture](#the-architecture)
  - [Long description](#long-description)
    - [What's the problem?](#whats-the-problem)
    - [The Idea](#the-idea)
    - [How can technology help?](#how-can-technology-help)
    - [How our product is better than exisitng solutions?](#how-our-product-is-better-than-exisitng-solutions)
  - [Project roadmap](#project-roadmap)
  - [Github Code Repositories](#github-code-repositories)
  - [Local Application Setup](#local-application-setup)
  - [Built with](#built-with)

## Short description

Sustainable future of our ecosystem , preserving wildlife and natural habitats.

## Demo Video

## The Architecture

![image](https://user-images.githubusercontent.com/25299400/122579914-0b0ab680-d073-11eb-9f71-9fa5adcd23ed.png)

1. Smart Collar Device collects animal's real time voice , current GPS location and weather data and send them to Python Server hosted on IBM Cloud.
2. The data will be processed using AI/ML models and returned back to Python Server.
3. The processed data will be sent to Kafka Producer hosted on IBM cloud Foundry.
4. The producer will produce the data to a topic using IBM Event Streams.
5. The consumer will consume the data using same topic.
6. The consumer will save the data in the database.
7. The data will be returned to the Python Server.
8. The collar monitor  will get the data from the Python server and displays.

## Long Description

### What's the problem?

The real problem here is the lack of information about state of wildlife where people aren't actively engaged to keep it sustainable. Around 1 million animals are threatened with extinction. It is found that health of ecosystems on which we and all other species depends is deteriorating more rapidly than ever. When a species becomes endangered, it is a sign that the ecosystem is slowly falling apart. The responsibility to keep these innocents life shouldn't just be on the shoulders of a few. Having such an engaging audience could improve impact, awareness and accelerate the drive towards sustainability.

### The idea

The idea is to build a technologically rich system to monitor the endangered species in real time and to spread awareness among people to save life on land. The system would be utilizing following with multifold solution.

### How can technology help?

- **Geolocation** : We have used a smart collar device tied to neck of endangered animals which will give us the location of those animals at every moment using GPS service. Those coordinates will be received by a front end application ,which are mapped and monitored continuously on google maps. As soon as the animal would come into a danger zone (where it could get harmed/poached) or if there is a risk of human-animal conflict (where it could harm the farms) , the  designated authority monitoring these collars would already know about it and could take necessary actions for that in time which would help us saving the animals from getting poached and also resolve human-animal conflict by keeping animals away from farms.
- **Real Time Weather (ML)** : We are fetching the real time weather of the animal's current location and make predictions about if the habitat is suited for that animal and how long that animal could survive in those climatic habitat.
- **Real time monitoring** : An application platform to monitor the live locations and dangers associated with the animals and notify authorities to take appropriate plan of action well within time when an animal is spotted in danger.
- **Social Platform** : A social platform to engage users to inform them about the endangered species using the data collected , spread awareness and promote them in helping to save Life on Land.
- **Voice Recognition Model** : We are collecting real time voice of the animals and running it over our voice recognition models and predict the chances of it being under threat.

### How our product is better than exisitng solutions?

There isn't any system available which would give us the real time data about the endangered animals as close as our system. Reason being , the Smart Collar will be attached to the animals and will receive the information about them much more accurately as compared to the Drones and even the robotic camera.

- Built on top of such a platform with multitude of applications which can deliver a rich experience to a user while providing some incentive like application giving a notification every time to the users about the number of endangered species left, maintaining natural habitat , protecting biodiversity and promote them to help saving the environment

## Project Roadmap

Following is our project roadmap, which depicts the current prototype listing of our system, and defines the future scope. 

![image](https://user-images.githubusercontent.com/25299400/122579972-19f16900-d073-11eb-9c27-74db226d9f0c.png)

## Github Code Repositories

Following are the instructions to run our project on the local machine for development and testing purposes, in a sequential manner.

- [Smart Collar](https://github.com/chhabrabhishek/Collar)
- [Collar Kafka](https://github.com/chhabrabhishek/collar_kafka)
- [Collar Monitor](https://github.com/chhabrabhishek/collar_monitor)

## Local Application Setup

1. Clone the [Smart Collar](https://github.com/chhabrabhishek/Collar) application, and follow the READ ME file to setup the application locally.
    - Or you can get the direct [APK setup](https://github.com/chhabrabhishek/Collar/blob/master/app-debug.apk) file, which you can install on your android phone and simulate the smart collar application.
2. Clone the [Collar Kafka](https://github.com/chhabrabhishek/collar_kafka) application, and follow the READ ME file to setup the kafka producers and consumers locally.
3. Clone the [Collar Monitor](https://github.com/chhabrabhishek/collar_monitor) application, and follow the READ ME file to setup the monitor application locally.

**Note** - All these steps must be done in a sequential manner to setup the code perfectly.

## Built With

- [Open Weather Map APIs](https://openweathermap.org/api)
- [Angular](https://angular.io/)
- [IBM Cloud Services](https://www.ibm.com/in-en/cloud/cloud-foundry)
- [IMB cloud foundry](https://cloud.ibm.com/catalog)
- [Flask (Python)](https://flask.palletsprojects.com/en/2.0.x/)
- [Google Maps](https://www.google.com/maps)
- [IBM MyBlue Mix Services](https://www.ibm.com/support/pages/overview-ibm-bluemix)
- [Kafka producer and consumer service](https://kafka.apache.org/)
- [IBM event streams](https://cloud.ibm.com/catalog/services/event-streams)

