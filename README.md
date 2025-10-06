

# 🧵 Multithreaded Server in Java

A **Multithreaded Server** built in **Java** that can handle multiple client connections simultaneously using the concept of **multithreading** and **socket programming**. This project demonstrates how a server efficiently manages concurrent requests without blocking communication.

---

## 🚀 Features

- Handles multiple client connections concurrently  
- Implements **TCP socket communication** (ServerSocket & Socket)  
- Uses **Java Threads** for parallel client handling  
- Thread-safe I/O operations  
- Logs client activity (connected/disconnected clients)  
- Scalable architecture for chat or data exchange applications  

---

## 🧠 Concepts Used

- Multithreading  
- Synchronization (if applicable)  
- Socket Programming (ServerSocket, Socket)  
- Input/Output Streams  
- Client-Server Communication Model  

---

## 📂 Project Structure

Multithreaded-Server/
│
├── src/
│ ├── Server.java
│ ├── Client.java
│
├── README.md

## ⚙️ How It Works

1. **Server Initialization**  
   The server starts and listens for incoming client requests on a specified port.

2. **Client Connection**  
   Each time a new client connects, the server spawns a **new thread** (via `ClientHandler`) to handle that client’s requests.

3. **Concurrent Communication**  
   Multiple clients can send/receive data concurrently without affecting others.

4. **Graceful Shutdown**  
   When a client disconnects, the corresponding thread terminates cleanly.

