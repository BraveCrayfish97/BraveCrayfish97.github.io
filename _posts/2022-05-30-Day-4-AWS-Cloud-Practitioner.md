## Day 4 of my Cloud Practitioner Certification
###### Today, I learned about DNS's role in networking and the different types of DNS routing that are available.

---

### What is DNS?
* Can be compared to a phonebook - translates domain name to IP adress
* User types domain name into search engine, then their DNS Provider goes out and finds the IP adress of the domain.
* Route 53 is the DNS provider by AWS 


---

### Types of DNS Routing
* Weighted
  * X percent of requests go to X IP and Y percent of requests go to Y IP
  * Used for beta testing
* Simple routing
  * Gives random IP from its list of possible IPs
* Geolocation routing 
  * based on the end user location - content customization based on the user country
* Latency routing 
  * gives the IP address that client has least ping for
  * fastest response
* Failover routing 
  * If the active IP address goes down, the passive IP address will be given.
* Multi Value routing 
  * returns multiple IPs and client picks one
