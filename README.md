# MultithreadApplication
Creating a MultithreadApplication in Java 

These proccess are there in the system. The operating system decides how to utilise a resource.The program itself cannot decide because we cannot 
give direct access to memory,otherwise it will be very unsecure. The program talks to the operating system .Now each of the process we make can have 
one or more thread.
In the old days,System use to have a single core so one thread can be executed at a single time.
In the old days,System use to have single CPU,so there time slicing was used  

Threads can be made by-
a).Extending Classes.
b).Implementing Runnable Interface.

Methods of the Thread Class-
a).Two constructor (default and one that creates a thread of the Runnable object)

b).Static method 
i).Sleep
ii).Yield

c).Instance Method-
i).Starts
ii)isAlive
iii).setPriority
iv).Join
v).Interrupt

