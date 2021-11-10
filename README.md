<h3 align="center"> Smart Car Parking System using Camera and Ultrasonic-Sensor with Computer Vision Techniques</h3>

 <p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/74568334/141007223-4ee9ffa4-772c-4cf9-be17-b3ac7cc92f20.jpeg">
</p> 

<h4 align="center"> <span style="color:green">SSD-Mobilnet/OCR/Keras/TensorFlow/OpenCV/Camera Fusion/RaspberryPi</span></h4>

<h3 align="left">Motivation </h3>
 
<p style= 'text-align: justify;'> As the current housing systems are moving towards automation, the focus on the systems used within the house is given more focus than the customer satisfaction. In addition, Home Vehicle parking system is one of the most important factors to reduce traffic and satisfy drivers. Moreover, when parking the vehicles in the apartment parking place, the driver has to open the door. So, the driver has to get out of the vehicle and open it. So the project objective is to develop a system to allow authorised vehicles in the particular apartment. Also, we used **computer vision** techniques and a **Raspberry-Pi camera** module and an **ultrasonic sensor** in order to make this system.</p>

<h2 align="center">Componentes Used for this Project</h2>

 <p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/74568334/141059484-9eff0664-dbd0-40dc-bf7e-c31214645540.jpg">
</p> 

<h2 align="center"> Technologies Used </h2>
 
 ```
 1. IDE - Pycharm
 2. SSD - Mobilenet - As a object detection model
 3. GPU - P-4000
 4. Google Colab - image alaysis
 5. OCR - Extract the numplerplate information
 6. OpenCV - Draw the bounding boxes
 7. RaspberryPi 4 - Run the program as a computer
 8. Joy-pi - Monitoting system
 9. Ultrasonic sensor - If any object detect by sensor and finding distance of the object from the sensor
10. Servo Motor - handling the door
11. MQTT - As a communication Protocol
 
 ```
  
 
 
<h3 align="left"> Project Limitations </h3>

 
<p style= 'text-align: justify;'> 
 
1.	Toy cars only used as vehicles
 
2.	**Two different cars** were used to demonstrate the project
 
3.	Just used **250 images** for each category to train the model
 
4.	Instead of the number plate, Pre-Defied number plate information was printed on white the paper
 
5.	The toy car was moved manually
.</p>


  
<h3 align="left">Sample Images</h3>

<p align="center">
  <img width="600" src="https://user-images.githubusercontent.com/74568334/140993929-60ec397c-79e7-489d-8dba-918315a3ae1b.jpg">
  <img width="600" src="https://user-images.githubusercontent.com/74568334/140993931-3d867c45-cce9-402d-8c8e-8628bbf0b073.jpg">
  <img width="600" src="https://user-images.githubusercontent.com/74568334/140993925-5cc30d5f-aa07-45a4-9062-8f708a73f54a.jpg">
</p> 

<h3 align="left">The process flow of this projects</h3>

<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/74568334/141005196-51f2be35-8c6d-46bf-9233-21fb8f22687e.png">
</p> 

 
<p style= 'text-align: justify;'> The above figure illustrates the Automated parking system for the smart home network. First, the vehicles model, number plate, and the name of the customer who lives in the apartment are collected and stored in a CSV file. To identify whether it was a car, motorcycle or vehicle, 500 toy car images were collected and trained on the SSD mobile - net model using the GPU-4000. Also, the trained model has later uploaded on rasperryPi4 Also, the camera module and Ultrasonic sensors were connected with raspberry. Subsequently, the ultrasonic sensor continues to work to detect and determine the distance of an object in front of the camera. If this distance is less than 10 cm, this information is published to the MQTT – Protocol to a particular topic. and To start the camera, it is giving a request to  MQTT with the same topic created by the ultrasonic sensor in MQTT and receiving the message from the ultrasonic sensor. In addition, the camera takes a picture and recognises from this picture whether it is a car or a motorcycle using SSD Mobel - net. It is the licence plate information that will be extracted if the licence plate already exists on the server, then the door will be opened.</p>

