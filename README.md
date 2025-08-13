# Chat-Application
Chat Application (Java Sockets) 💬
This is a simple client-server chat application developed in Java, demonstrating the use of sockets for communication.

Features ✨
Client-Server Architecture: Utilizes a dedicated server to handle connections and message routing between multiple clients.

Real-time Messaging: Clients can send and receive messages instantly.

Multi-client Support: The server can concurrently manage connections from multiple chat participants.

How it Works 🛠️
The application leverages Java's java.net.Socket and java.net.ServerSocket classes to establish and manage network connections.

Server:

Listens for incoming client connections on a specified port.

For each new client, it creates a dedicated thread to handle communication, ensuring non-blocking operations for other clients.

Receives messages from clients and broadcasts them to all other connected clients.

Client:

Connects to the server's IP address and port.

Sends messages to the server.

Receives messages from the server (which were broadcast by other clients).

Getting Started 🚀
Prerequisites
Java Development Kit (JDK) 8 or higher installed on your system.

Running the Application
Clone the Repository (or download the source code):

Bash

git clone <repository_url>
cd <repository_directory>
Compile the Java Source Files:
Open a terminal or command prompt in the project's root directory and run:

Bash

javac *.java
Start the Server:
First, launch the server application:

Bash

java ChatServer
The server will start listening for connections on a default port (usually 12345, though this can be configured in the ChatServer.java file). You'll see a message indicating the server is running.

Start Client(s):
Open a new terminal or command prompt for each client you want to run. Then execute:

Bash

java ChatClient
The client will attempt to connect to the server. Once connected, you can start typing messages in the client window.

Project Structure 📁
ChatServer.java: Contains the server-side logic for handling client connections and message broadcasting.

ChatClient.java: Contains the client-side logic for connecting to the server, sending messages, and receiving messages.

(Optional: Other utility files if present in the project)

Contributing 🤝
Feel free to fork this repository, suggest improvements, or submit pull requests. Any contributions are welcome!

License 📜
This project is open-source and available under the MIT License.
