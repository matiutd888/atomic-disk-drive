# Atomic Disk Drive

Atomic disk drive that stores data in fault-tolerant distributed register.

Project for Distributed Systems course at the University of Warsaw (I am proud to say my solution was the only one that received a perfect score) 

A distributed register consists of multiple processes running in user space, possibly on multiple physical (or virtual) machines. 
A Linux block device driver communicates with the processes using TCP. The processes themselves communicate using TCP too. The processes can crash and recover at any time.

Each Atomic Register process uses tokio to handle multiple requests asynchronously 

Atomic disk drive and its modules are best explained in the diagram below (everything besides the driver had to be implemented)

![output-onlinepngtools](https://user-images.githubusercontent.com/34310650/217945330-1dcb27d2-9b1f-44fa-8317-24b6c7c9a7b3.png)
