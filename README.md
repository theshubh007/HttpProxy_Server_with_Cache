
# HttpProxy_Server_with_Cache

This project implements a high-performance, multi-threaded HTTP proxy server with LRU (Least Recently Used) caching functionality. Designed for scalability and efficiency, it excels at handling a high volume of concurrent client requests, specifically focusing on GET requests for this initial implementation.

## Key Features

- Scalable Threading: It includes **multithreading** for efficient concurrent client connection management, maximizing server throughput. 

- LRU Caching: Optimizes performance for frequently accessed URLs by implementing an **LRU** cache with customizable capacity and eviction strategy. 

- Robust Error Handling: Gracefully handles various error scenarios like invalid requests, connection failures, and internal server errors, providing informative error responses to clients using well-defined HTTP status codes.

- Cross-Platform Compatibility: Leverages **standard C libraries (pthread, socket)** for broad compatibility across different operating systems.

## Technical Specifications

- Language: C 
- Concurrency Model: Multithreading using POSIX threads (pthread)
- Networking: TCP sockets
- Caching: LRU implementation (customizable size and eviction policy)
## API Reference

#### Follow this commands to test this project

1. Clone this project in your device
```
  git clone https://github.com/theshubh007/HttpProxy_Server_with_Cache.git
```
2. This automates the execution of build instructions based on dependencies specified in the Makefile.
```
  make
```

3. Start the proxy server on port 8080:
```
  ./proxy XXXX( replace X with any port eg.8080)
```


4. As next step call the GET request

```
http://localhost:XXXX/https://www.cs.princeton.edu/
(Replace XXXX with previously entered port eg.8080)
(This princeton website follows GET request category, that's why we're testing on it)
```


## Project Output:


![Screenshot 2024-06-30 171151](https://github.com/theshubh007/HttpProxy_Server_with_Cache/assets/100220928/a6986b5b-734a-4c44-8f41-c49283a523cd)




