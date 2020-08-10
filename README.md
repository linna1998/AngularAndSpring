# Student Event Engagement Portal

Authors:   Ke (Lina) Ding, Madhusmita Dash, Mengyu (Mia) Zhang, Xinyi He					

## Problem Statement (Theme: STEM+Covid-19)

1. Covid-19 outbreak all over the world
2. Students study remotely may suffer from loneliness and depression
3. Lack of interaction among students both for studies and leisure
4. Interact with new students and get engaged in the portal

## Project Significance

1. Provide an online platform for students to get engaged in events
2. Help protect mental and physical health of students under this tough time
3. Propose a new format of online education and entertainment

## Tech Stack
1. Front end: Angular.JS
2. Backend: SpringBoot + MongoDb
3. Deployment on Kubernetes using Kind

## Project Overview
1. Student Login Page
2. View my profile page: 
    - View the list of events created by me
    - View the list of events subscribed by me
    
3. Events page:
    - View the upcoming events for each category
    - Select an event and join the link 
4. Category of events:
    - Wellness 
    - Study
    - Virtual Coffee Chats
    - Games
    - Random

## Commands to build and run
```
./mvnw package && java -jar target/angularandspring-0.0.1-SNAPSHOT.jar
docker build --build-arg JAR_FILE=angularandspring-0.0.1-SNAPSHOT.jar -t test .
docker tag test mdash95/angularandspring
docker push  mdash95/angularandspring
kubectl port-forward angularandspringpodname 8081:8080
```


