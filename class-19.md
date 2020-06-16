# Namespaces

Socket.IO allows you to “namespace” your sockets, which essentially means assigning different endpoints or paths.

This is a useful feature to minimize the number of resources (TCP connections) and at the same time separate concerns within your application by introducing separation between communication channels.


# Default namespace

We call the default namespace / and it’s the one Socket.IO clients connect to by default, and the one the server listens to by default.


# Rooms
Within each namespace, you can also define arbitrary channels that sockets can join and leave.



[Home Page](https://osamamousa204.github.io/reading-notes-401/)