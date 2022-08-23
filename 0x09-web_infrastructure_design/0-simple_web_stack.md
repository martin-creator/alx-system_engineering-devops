##0. Simple Web Stack
The simple web stack is the simplest form of web architecture that is made up of one of the following components:
1. 1 server
2.  web server (Nginx)
3. 1 application server
4. 1 application files (your code base)
5. 1 database (MySQL)
6. 1 domain name foobar.com configured with a www record that points to your server IP 8.8.8.8

This form of web architecture is situated for simple web applications as it relatively simple to setup and  its availability suites basic amplications where scalability and high availabilty is not a top priority. 

####What is a server?
Servers are physical machines (as hardwares), virtual machines or softwares (computer programs) that serve or provide functionality to other programs or devices called “clients”. 
It is worth noting that a computer can function as a server, and a server can be a computer, both of them being built up with hardware and software. The main difference comes in when we try to compare the storage capacities and processing powe, where serves outshine their counterparts. It is said that servers are computers on steriods!
Examples of servers include: 

####What is the role of the domain name?
The domain name  replaces complex alpanumerical IP addresses  into easily understandable/memorable names that humans can remember and communicate easily. In otherwards, domain names are some sort of abstraction away from machine code. 

####What type of DNS record www is in www.foobar.com?
DNS record of www belongs to a subdomain of the www.foobar.com.  Remember that the parent domain  is foobar.com. 

####What is the role of the web server?
Web servers make web hosting possible because they provide storage space for the  program source files. The main function of a web server is to store the files of a site and broadcast them over the Internet so that they can be visited by users. Web servers mainly manage static files that don't change. 

####What is the role of the application server?
The application server is the intermediary between browser-based databases and back-end databases and legacy systems. The backend logic of the applications servers is stored on the application server which has direct access to the database. 

####What is the role of the database?
Databases organizes data so  it can be easily accessed, managed and updated. There are many types of database that are categorized according to the way they store and manipulate data. 

1. Relational databases: Are composed of a set of tables where data is organized into a predefined category. 
2. Distributed database: Distributed database system consists of portions of a database that can be heterogeneously or homogeneously distributed along multiple physical locations.
3. Cloud database: Cloud database is a database built in a virtual environment, just as in a hybrid cloud, public cloud or private cloud.
4. Object-oriented database: Another example is an object-oriented database which is organized around objects instead of actions. 

####What is the server using to communicate with the computer of the user requesting the website?
The server is using the HTTP (Hypertext Transfer Protocol), which enables the transfer of resource and data, such as HTML documents between the server and the client.  Clients send requests and Servers send reponses. 

####Issues with the simple web infrastructure
1. This infrastructure has a SPOF (Single Point of Failure) where if component of the system fails, there is no backup that can support the continuity of the functionality of the system, bringing the whole system to a collapse by being unable to operate.
2. Whenever some structure or node in the system needs to be repaired, the whole system has to be shut down, while the maintenance is done. Then, client requests cannot be attended during this period of time.
3. Overload of traffic can be a risk to the server capacity. This, because there is no possibility to scale the service with additional servers as backup. Leading to a possible breakdown of the web page and client requests, as traffic surpasess servers capacity.(This infrastructere is very prone to Denial of Service Attacks)

