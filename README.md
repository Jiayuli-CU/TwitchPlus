# A Personalized Twitch Resources Recommendation Engine

## I. Introduction
<p justify-content="space-between">In this project, we designed and build a full-stack web application for users to search resources on Twitch, including streams, videos and clips, and get recommendations based on their favorite collections or the top games on Twitch. The application supports funtions including register, login/logout, search, add collection, and get recommendation. All relative game recources for this project are directly retireved from Twitch.tv by APIs officially provided for developers, and a content-based algorithm is implemented for recommendation. After development, the service is deployed to AWS EC2 for better performance. Load test is also conducted for further optimization.</p>

## II. Frontend Development
<p justify-content="space-between">The frontend of this application is built with React and And Design. React is modulized and can efffectively render the webpage with its virtual DOM, while Ant Design provides various high-quality UI components. The final design of the web pages are shown in Fig. 1-4 below.</p>

<div align="center"><img src="https://github.com/Jiayuli-CU/TwitchPlus/tree/main/Pics/homepage.png"></div>
<p align="center">Fig. 1 Home page</p>

<div align="center"><img src="https://github.com/Jiayuli-CU/TwitchPlus/tree/main/Pics/register.png"></div>
<p align="center">Fig. 2 Register</p>

<div align="center"><img src="https://github.com/Jiayuli-CU/TwitchPlus/tree/main/Pics/login.png"></div>
<p align="center">Fig. 3 Login</p>

<div align="center"><img src="https://github.com/Jiayuli-CU/TwitchPlus/tree/main/Pics/recommendation.png"></div>
<p align="center">Fig. 4 Get Recommendation by Favorite Records</p>

## III. Backend Development
<p justify-content="space-between">The backend of this application is developed based on JavaEE platform, which provides API and runtime environment for developing and running large-scale, multi-tiered, reliable, and secure network applications. For each of the functions mentioned above, a corresponding Java Servlet is utilized to implement RESTful APIs and extend the capabilities of the Apache Tomcat server that host this application. The structure of the backend is shown in Fig. 5.</p>

<div align="center"><img src="https://github.com/Jiayuli-CU/TwitchPlus/tree/main/Pics/backendStructure.png"></div>
<p align="center">Fig. 5 Backend Structure</p>

<p justify-content="space-between">The data relevant to user information, game recources, and favorite records are stored in MySQL database. The ER diagram of the database is shown in Fig. 6.</p>

<div align="center"><img height="300" width="600" src="https://github.com/Jiayuli-CU/TwitchPlus/tree/main/Pics/SQL.jpeg"></div>
<p align="center">Fig. 6 ER Diagram of the Database</p>

## IV. Load Test & Optimization
<p justify-content="space-between">To improve the performance of the web application, we deployed it to AWS EC2. We also conducted load test and measured its QPS with Apache JMeter for further improvement. An optimizaion is implemented by applying the DBMS connection pool provided by Tomcat. The QPS increased 13 times after the optimization by comparing the load test results. The results are shown in Fig. 7. </p>

<div align="center"><img height="250" width="625" src="https://github.com/Jiayuli-CU/TwitchPlus/tree/main/Pics/loadTest.png"></div>
<p align="center">Fig. 7 Load Test Results</p>

