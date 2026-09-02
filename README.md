# TCP Client-Server Application

A TCP client-server application written in C++ using the POSIX Socket API.

The project was created as a practical exercise in network and system programming on Linux/Unix systems.

## Features

### Server

- Creates a TCP socket
- Binds the socket to a local address and port
- Listens for incoming connections
- Accepts client connections
- Handles clients in separate processes using `fork()`
- Handles terminated child processes using `SIGCHLD`
- Uses `waitpid()` to prevent zombie processes

### Client

- Establishes a TCP connection with the server
- Sends data to the server
- Receives server responses
- Uses `select()` to monitor both standard input and the network socket

## Technologies

- C++
- TCP/IP
- POSIX Socket API
- Linux/Unix system calls
- Processes
- Signals
- `select()`

## What I practiced

While working on this project, I practiced:

- TCP client-server communication
- POSIX socket programming
- Process creation with `fork()`
- Signal handling
- Multiplexed I/O using `select()`
- Working with Linux/Unix system calls
