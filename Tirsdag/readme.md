Fundamental Network Topics

Understanding Basic Network Terms like IP, TCP/IP, DNS, DHCP and more.
These exercises are meant to be answered with text, based on internet searches so write down your reply so you will remember for later.

What is your public IP address right now, and how did you find it? 

Public IP adresses can be found by all. The IP is used to communicate with other devices. 

The IP adress can be found in several different ways (MacOS) :

The easiest way is to ”ask” a website, as it can see your public adress: 
            https://whatismyipaddress.com
ifconfig |grep inet. In terminal 
Under network settings – advanced – TCP/IP 


What is your private IP address right now (do this both at home and in school), and who/what gave you that address?

The local router assigns the private IP address.  The same steps as before, can be used to find the private IP adress. 

What’s special about these address ranges?
 10.0.0.0 – 10.255.255.255
172.16.0.0 – 172.31.255.255 
192.168.0.0 – 192.168.255.255

The internet Assigned Numbers Authority (IANA) have reserved these address blocks for use as private IP adresses.  The first block allows 16 million addresses, the second over 1 millon and the last over 65.0000 


What’s special about this ip-address: 127.0.0.1?

Is is a reserved IP address, like the private, in the sense, that it is more limited than that. 

It is called a loopback address, and can be used to test network adaptors and integrated chips. Also called localhost. The address is used to establish an IP connection to the same machine or computer being used by the end user. 


What kind of service would you expect to find on a server using these ports: 22, 23, 25, 53, 80, 443?

A full list of services can be seen in this link:

https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers 


What is the IP address of studypoints.info and how did you find it?

In terminal write the command : ping www.studypoints.info

PING www.studypoints.info (157.230.21.145): 56 data bytes.

If you write https://studypoints.info in your browser, how did “it” figure out that it should go to the IP address you discovered above?

The DNS server knows the IP number of every website, 


Explain shortly the purpose of an ip-address and a port-number and why we need both

The IP address handles the connection between devices and the destinationpage. It is unique. The ports are what services, these connections are handling. So like a key to a door. 

What is your (nearest) DNS server,?

The nearest DNS server, can be used instead of the default one, if you want a safer and faster experience.

Can be found by downloading DNS Benchmarks or other. 


What is (conceptually) the DNS system and the purpose with a DNS Server?

It is like the phone numbers of the internet. It enables us to not remember the IP numbers of every website, but only the website name. 

What is your current Gateway, and how did you find it?

A gateway IP refers to a device on a network which sends local network traffic to other networks. Can be found in the same network settings, as the IP address earlier. 

What is the address of your current DHCP-Server, and how did you find it?

Command in terminal or see in network settings. 

ipconfig getoption en0 server_identifier

Explain (conceptually) about the TCP/IP-protocol stack

It is a protocol that describes how to hosts talk together (computer A and computer B).
The communcation travels through 4 layers of protocol (7 in the OSI model). Application, transport, internet and network access.  The sum of these stack enables computer A to talk with computer B. Each layer knows nothing of the underlying layer.  It is in the internet layer, that IP adresses are given, which sends it to the network acess layer (which have a MAC address). 


Explain about the HTTP Protocol (the following exercises will go much deeper into this protocol)

HTTP is the foundation of data communication on the internet, through requests and responses with browsers and serveres. 



Explain (conceptually) how HTTP and TCP/IP are connected (what can HTTP do, and where does it fit into TCP/IP)

HTTP works at the application layer and implements communication between a client and a server. These messages are delivered through TCP/IP connections. http defines how commands and responses are formatted and delivered. 

