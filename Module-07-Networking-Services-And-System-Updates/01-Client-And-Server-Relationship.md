## Client and Server Relationship

A **client-server relationship** is a communication model where a **client** requests services or resources, and a **server** provides them.

### Client
- Initiates requests
- Usually a user-facing application (browser, SSH client, mail client)
- Examples: Web browser, PuTTY, curl, Outlook

### Server
- Listens for incoming requests
- Processes requests and sends responses
- Examples: Web server (Apache, Nginx), SSH server, Mail server

### How It Works
1. Client sends a request to the server
2. Server processes the request
3. Server sends a response back to the client

### Common Protocols
- **HTTP/HTTPS** – web communication
- **SSH** – remote server access
- **FTP/SFTP** – file transfer
- **SMTP/POP3/IMAP** – email services

### Key Characteristics
- Centralized control on the server
- Multiple clients can connect to one server
- Communication usually occurs over a network

### Example
A web browser (client) requests a webpage from an Nginx server (server), which responds with HTML content.
