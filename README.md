# Math-bot

## Overview
Implement a network client that will communicate to a remote server in the C programming language base on [tutorials](https://www.binarytides.com/socket-programming-c-linux-tutorial/). The server implements a simple protocol that requires your client to send your netid@umass.edu email. After you do this then the server will respond to your client with a series of simple math problems that your client will need to solve.
- Network System Calls: Using system calls in order to communicate to the network. These are special functions that act as an API to the kernel and the operating system. You should take a look at this [post](http://linasm.sourceforge.net/docs/syscalls/network.php) to see a list of network system calls that are used in building networked applications. In addition I use 
these [structures](https://www.tutorialspoint.com/unix_sockets/socket_structures.htm) as parameters and return values for these system calls.
- Networking: This project will use a network socket, which is a special file descriptor that allows user to interface the networking stack. 
As explained in class, computer networks are organized in layers. The sockets we will be using here will allow user to interact with the transport layer of the stack. 
More specifically, I will be using [TCP stream sockets](https://en.wikipedia.org/wiki/Network_socket).

## How to run
After downloading the file, you can run this line in the terminal. We will be running a test server at address 128.119.243.147 on port 27993:
- $ ./client netid@umass.edu 27993 128.119.243.147

