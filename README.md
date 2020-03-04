# Multithreading-Server
Made a Multithreading Server Project for Operating System Course

## Description
I have created a multithreaded server with N threads by requesting from the server.  When a new client request arrives, the server will add it to a queue of connections. The threads will remove one connection from the queue and will handle the request. If the connection queue does not have a connection available, the thread will “sleep” until a connection is ready. The program should not use busy waiting.


## How to Run the Code(For Linux System)

1- make sure you cloned it in your local directory or do it by 

```console
local:~$ git clone https://github.com/RituRajSingh878/Multithreading-Server.git
```
2- go into Multithreading-Server directory and type the following command
```console
local/Multithreading-Server:~$ make
```
3- to run the server type the following command
```console
local/Multithreading-Server:~$ ./server
Usage: ./server port number_of_threads size_of_connections_array

```
It will show the above output in your command line and it is asking for the port and 
no. of threads to initiate and size of the connections array. So make sure you are giving it the proper inpute formate.
eg.
```console
local/Multithreading-Server:~$ ./server  8080 10 50
 ```
 After giving this command, local server is running inside your computer. Now You have to run a clint server without closing this server so open a new terminal in the same directory and run the following command.
```console
local/Multithreading-Server:~$ ./client 127.0.0.1 8080 50
[output] Result is 500
 ```
