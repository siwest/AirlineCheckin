AirlineCheckin
==============
A Java Queue implementation
An assignment for NJIT 610 Fall 2014 class.

Build an implementation of a queue ADT.
Use this implementation to build a simulation of waiting queues at an airline check-in counter, organized as follows:
There are two types of passengers: first class, and coach.
There are two service stations for first class, and three for coach.
There is a single queue for each type of passenger (first class, coach).
Passenger arrival times are random and are generated by a random number generator.
Average arrival rates for passengers are R1 for first class and R2 for coach. These are decided at run-time by prompting the user.
Service time is random and varies uniformly between 1 and S1 for first class, and between 1 and S2 for coach. Parameters S1 and S2 are also determined at run-time, by prompting the user.
Whenever a service station is available and the corresponding queue is not empty, we pick the passenger at the front of the queue and place her/him on the service station.
Whenever a first class service station is available and the first class queue is empty, the service station may service a passenger from coach.
The duration of the experiment, in minutes, is decided by the user at run time.
Statistics generated by the simulation include: average service time, maximum service time, number served in each class, maximum queue length for each type of passenger.

==================================================================================================================================

There are six Java classes supporting the Airline Checkin process. 
  The Simulator class contains the main method to run the program and develop test cases.
  The AirlineCheckinQueue class contains the basic Queue abstract data type (ADT).
  The Passenger class contains information about whether the passenger is first class or coach, the arrival time, time in queue, 
  and time at the service desk.
  The ServiceAgent class adds passengers, calculates a pseudo-random time to complete "servicing", and removes the passenger.
  The ServicedPassenger class keeps records on how long each passenger was served and a running max and average of all added 
  passengers.
  The Clock class keeps all the static methods syncronized for the Simulator.





TODO:
-Work on array overflow exceptions in AirlineCheckinQueue, ServicedPassengers, and the Simulator. Consider changing array indexing variable type from int to float say that we can access a greater set in the Queues/arrays at any time.
...

