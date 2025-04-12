Multithreaded Web Server (Server and Client)
This project demonstrates a simple multithreaded web server-client application in Java. The server listens on a specific port and handles multiple client connections concurrently using threads. The client sends a message to the server and receives a response.

Project Overview
Server Class: A simple multithreaded server that listens for client connections on a specified port. Each client connection is handled by a separate thread, allowing the server to manage multiple clients simultaneously. The server sends a greeting message to the client and logs the connection information.

Client Class: A client that connects to the server, sends a message, and receives a response from the server. The client runs in a loop, creating multiple threads to simulate multiple clients connecting to the server.

Features
Multithreading: Each client is handled in a separate thread on the server side, allowing the server to handle multiple client requests concurrently.

Socket Communication: The server and client communicate using TCP sockets.

Timeout Handling: The server has a timeout feature, automatically closing connections that are idle for too long (set to 70 seconds).

Client Simulation: The client creates 100 threads, each simulating a separate client making a request to the server.

How It Works
Server
The server listens for incoming client connections on port 8010.

Upon accepting a connection, the server spawns a new thread to handle the client request.

Each client receives a greeting message with the client's IP address.

The server runs indefinitely, accepting new client connections.

Client
The client connects to the server using the IP localhost and port 8010.

It sends a greeting message with the client's local socket address.

The client waits for a response from the server and prints it to the console.

The client creates 100 threads, simulating multiple clients connecting to the server.

Requirements
Java 8 or higher

IDE (like IntelliJ IDEA, Eclipse) or command line to run Java programs

How to Run
Step 1: Run the Server
To start the server, run the Server.java class:

Step 2: Run the Client
To run the client, compile and execute the Client.java class:


