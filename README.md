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

ThreadPools are the way to regulate thread in an application without needing to manually start each thread to start a thread for each task.
Java uses the executor interface for executing task in the Thread pool.

Executor service is the sub interface of the Executor.
We will use executor static method to create a new executor object. 

AtRuntime , its going to decide which thread is going to run.


RaceConditions-
Race Conditions are the major source of trouble when dealing with the multithreaded Application.

Whats a race condition here ?
A race condition is condition when two threads are trying to modify the same memory object, and depending on the ondering
on which they are executed we will get different results
In our Banking Application this can occur whenever we have different thread trying to modify a 
the same account balance at the same time.


To avoid race Condition we have to snchronize the thread.
Thread synchronization allows us to that one thread can simultaneously access a certain 
part of program.
The region is called critical section
A method ,loop or any block of code that can be deemed synchronized.

When we are trying to access the sysnchronized text remember that other threads have to wait .

for instance method,the synchronization occurs on the object.
for static method , the synchronisation occurs on the class.

Synchronised will read the correct info . but we are not sure whether she will be able to update that info or not .
For that we need to coorporate with thread.

Locks Basics-
a).When we synchronoze a section of code,each thread acquire a lock on the object or class.Executes the coe and thn releases the lock.
for another class to access the lock , we need access of lock.

Lock is an interface,Rentric lock is a concrete.
Each lock must have the fairness policy-
if fairness is true,the longest waiting thread will get the lock next.


There are few conditions of locks-
Await-It causes the locks to wait until he gets signalled 
Signal-Wakes up the Waiting Thread
SignalAll-Wakes up the waiiting thread.

-if we don't explicitly signal a thread ,the thread will die and starves
-Essence-Sometimes we pass locks between theards to prevent lock conditions but sometimes the thread does not get 
the CPU time .





 












































