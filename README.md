# Client-Server-socketProgramming
Introduction 
In this assignment, we use sockets to implement a simple web client that communicates with a web server using a HTTP which is an application layer protocol. 
The Multi-threaded Web Server:
The web server  accepts incoming connection requests then, if it is a GET request it  picks out the name of the requested file and call “GET_handler” function to Handel the request,If the request is POST then it sends OK message and wait for the uploaded fille from the client. 
 Functions:
Get_handler(data): It takes the command and handles get requests .It checks if the file is found it sends the data and 200 OK in the status code if not found 404 file not found 
Post_Handler(data):  It takes the command and wait for the client to send the file. 

Command to run the server : 
        py /server.py  port_number 
Why multi-threading?
we used multi-threading to handle multiple connections because our project  is network bound  because many scripts related to network/data I/O spend the majority of their time waiting for data from a remote source. 

The HTTP Web Client :
Our web client reads and parse commands from the standard input. And handles the POST and GET commands 
The commands syntax should be as follows: 
GET file-name host-name http version
POST file-name host-name  http version



Functions:
Get_handler(data): It receives the data from the server
Post_Handler(data): It sends request to post file and sends the file 
Command to run the client : .
        py /client.py  ip number port_number 
 
Our project handles HTML, TXT and images. 


