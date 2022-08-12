# multimodalDataRecording

Package for multimodal (text based haptic and audio) data capture for ROS applications. 
It consists of generic subscribers, which are nodes that record data about generic ROS topics and stores them in a .csv file. 
The number of topics and topic names should be provided to the "numTopics" and "topicName1, topicName2, topicName3..." arguments of the "recordingService.launch" file. 
The audioRecorderNode is launched automatically along with the genericDataRecordingNode(s) and starts recording audio from the default input PCM device when the client nodes sends the service request to the recorderServer node. 

Example of bringup, and resulting ROS graph: 
![image](https://user-images.githubusercontent.com/107273918/184397195-1a1eb534-0ab2-405b-8026-bb51026f30e4.png)

