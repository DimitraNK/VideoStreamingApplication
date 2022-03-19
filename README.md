# VideoStreamingApplication
This video streaming application is inspired by TikTok. It allows users to upload and download video content.   
Three broker nodes and two appnodes were used. Every node has a different port.
The dataset for the application can be found at 
https://drive.google.com/drive/folders/19Vxb4-3Ler8GnB1vwjBDvUD14rGV95Yp?usp=sharing
and it contains a folder for each publisher, within which there is a video and its corresponding txt 
document that has all the hashtags for that video.
Any other dataset can be used as long as it is placed within the folder of the project files, and its name,
as well as its subfolder names are the same as the original dataset.  

In order for this project to be compiled and run, Visual Studio Code was used. The three brokers use ports 200,
888, 4675, and the broker that uses port 200 is the main broker, which means it is respondible for 
communication between the appnodes; which are content producers and consumers. The two appnodes channel names
are channel_name1 and channel_name2. In order to run the code in a computer the ip address should be replaced
with the computer's ip. A terminal for each of the brokers and publishers should be opened (5 terminals in
total), and for the brokers the command is of the following format: java Broker ip_address port_number,
where ip_address and port_number should be replaced with the ip and port number for the broker.
For the publishers, the command is: java Publisher ip_address channel_name, where ip_address and channel_name
should be replaced with the ip and the channel name.
