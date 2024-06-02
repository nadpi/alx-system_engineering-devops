Infrastructure Details:

-What is a server?
A server is a software or hardware device the provides a specific service for a client.

-What is the role of the domain name?

*domain name in a nutshell:
Imagine a phonebook, the domain name corresponds to a specific person’s name and the IP address that is assigned to that domain name corresponds to the phone number of that person.

-What type of DNS record www is in www.foobar.com?
Type of DNS record: Canonical Name (CNAME)
One can use CNAME records to point www.foobar.com to the DNS entry for foobar.com, which in turn has an A record which points to the IP address.
An A record maps a domain name to the IP address (Version 4) of the computer hosting the domain.

-What is the role of the web server?
A Web Server handles the HTTP requests received from a client.

-What is the role of the application server?
An Application Server exposes business logic to client applications through various protocols, possibly including HTTP.

-What is the role of the database?
The database store the site’s data. 

-What is the server using to communicate with the computer of the user requesting the website?
HTTP protocol


Issues with this infrastructure:

-SPOF (Single Point of Failure):
If there is a flaw in the design configuration or implementation of a system or component poses a potential risk because it could lead to a situation in which just one fault causes the whole system to stop working. if there is any flaw in one of the server components such as web server, DB engine, etc., the whole system will stop working and the system won’t available for the authorized clients.
-Downtime when maintenance needed (like deploying new code web server needs to be restarted)
it’s a period during which a system is unavailable because there is ongoing maintenance happening. To avoid this issue, another server is needed in order to keep the flow going and make the system always available.
-Cannot scale if too much incoming traffic
To avoid this issue, other server should be added to distribute the traffic to these servers, and a load-balancer to distribute it.








