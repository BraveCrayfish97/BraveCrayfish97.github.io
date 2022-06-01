## Day 3 of my Cloud Practitioner Certification
###### Today, I learned about the relationship between the responsibilities of AWS and the Customer. I also explored in depth the advantages of using a LoadBalancer to direct traffic and also the various types of LoadBalancers AWS provides us with.

---

### AWS vs the Customer Responsibilities
* AWS Responsibilites
  * Security “of” the cloud
  * Physical security
  * Firmware upgrade on networking devices
* Customer Responsibilties
  * Security “in” the cloud
  * Managing security groups and network ACLs
  * Creating IAM users and setting password policies

---

### Advantages of using a LoadBalancer
* Traffic is not routed to deffective servers
  * AWS ELB runs keepalive checks on its EC2 instances and won't send traffic if checks come back negative
* Distributes traffic across its EC2 Instances


---

### Types of Load Balancers
* Classic LB
  * supports layer-7 http and layer-4 tcp
  * legacy type
* Network LB
  * supports only layer-4 tcp
  * used for high speed requests that don't have user dependent responses

* Application LB
  * supports only layer-7 http
  * used for most websites - take in headers and other info 
