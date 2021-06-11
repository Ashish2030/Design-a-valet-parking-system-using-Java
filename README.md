# Design_a_valet_parking_system_using_Java

Problem statement 
===================
Design a valet parking system. Requirements of the valet parking system are:  
1. Parking lot is fixed in size and cannot be over parked.  
2. A vehicle is allowed only when a suitable parking spot is available.  
3. Customers are given a ticket that they can use to redeem to get their vehicle back.  
4. Parking spots come in three sizes, small, med, large  
5. Thee types of vehicles, small, med, large can be parked  
	i. Small vehicle can be parked in a small, medium, and large spot  
	ii. Medium vehicle can be parked in a medium or large spot  
	iii. Large vehicle can be parked only in a large spot

Design and assumptions
=======================
Resources in the system have been identified and translated to java classes directly to design this modularilzed and extendable valet parking system. Composition has been used extensively for enabling re-usability, de-coupled classes, and easy unit-testability. No. of Unit test cases have been written to give us a safety-net to rapidly refactor, add frameworks and extend the application. Spring, Hibernate, Maven have not been used as the intention here is to just show the design aspects and to deliver the prod ready code in a very quick time. Database/Dao layer is not present but application's entities could be directly mapped to DB tables. Because of composition's heavy usage, it would be a matter of couple of hours to convert it into a full fledged spring/hibernate based application. At last, Concurrency aspect has been left out to keep things simple at this point of time. A simple Runnable 'ParkTheCarTask' is present however just to show the intention of not keeping the customer waiting for the valet token after giving the car to the ValetParkingManager.

