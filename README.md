# Simple GUI based Chat Application

This is a simple GUI-based chat application implemented in Python. The application allows users to connect to a chat server, send messages, and receive messages broadcasted by the server. It provides a user-friendly interface using the tkinter library.

## Features

- Connect to a chat server and exchange messages with other connected clients

- Choose a nickname to be displayed alongside sent messages

- Real-time chat experience with messages displayed in the GUI

- Responsive and interactive GUI with message input and chat history

## Prerequisites

- Python 3.x

- tkinter library (usually comes pre-installed with Python)

## Usage

1. Run the server:
   - Open a terminal or command prompt and navigate to the server directory.

   - Execute the following command:
     ```
     python server.py
     ```

2. Run the client(s):
   - Open a terminal or command prompt and navigate to the client directory.

   - Execute the following command:
     ```
     python client.py
     ```

3. Use the GUI:
   - The client GUI will open, prompting you to enter a nickname.
  
   - Enter a nickname and click "OK" to connect to the server.
   
   - Once connected, you can enter messages in the input area and click "Send" to send them to the server.
   
   - Received messages from other connected clients will be displayed in the chat history area.
   
## Technical Details

-	The application uses the socket module to establish a network connection between the client and server.

-	It utilizes the threading module to enable concurrent execution of the GUI and message receiving functions.

-	The GUI is built using the tkinter library, which provides a user-friendly interface for the chat application.

-	The chat application follows a client-server architecture, where multiple clients can connect to a central server and exchange messages.

-	Clients can choose a nickname upon connection, which will be displayed alongside their messages in the chat.

-	The server runs on a specific host and port (in this case, '127.0.0.1' and 9090).

-	The client application connects to the server by creating a socket and establishing a TCP connection.

-	The client's GUI is created using tkinter, with labels for chat history and message input, a text area for displaying chat messages, and a send button.

-	The client GUI is responsive and interactive, allowing users to enter messages and send them to the server.

-	Messages sent by the client are encoded as UTF-8 strings and sent over the socket connection to the server.

-	The server receives messages from clients, decodes them, and broadcasts them to all connected clients.

-	The server keeps track of connected clients and their respective nicknames.

-	The server uses multi-threading to handle multiple client connections concurrently.

-	Chat messages received by the client are displayed in the text area of the GUI, providing a real-time chat experience.

-	The client application can be closed by the user, which will gracefully terminate the client's connection with the server and close the GUI window.


