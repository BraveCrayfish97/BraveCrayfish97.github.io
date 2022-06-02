## Day 6 of my Cloud Practitioner Certification
###### Today, I learned about the AWS Networking fundamentals and also about the role of security groups and network access control lists.

---

### AWS Networking Fundamental Concepts
* VPC
  * functions as a virtual network that is spread across a region
  * all instances within one VPC can communicate with each other via private IP
* Subnets
  * subdivisions within a VPC
  * can be public (has route to IG) or private (doesn't have route to IG)
  * if public, all instances within get a public IP
  * at the AZ level
* Internet Gateway
  * similar to router for a home
  * connects VPC to internet
* Route tables
  * has rows in which set of IPs go to specfied location.
  * one subnet cannot have more than one route table.
  * If a subnet has a connection to IG in its route table, it is considered a public subnet, and all instances within that subnet are given public IPs.


---

### Security Groups vs Network Access Control Lists
* Security groups
  * at instance level
  * can create ONLY list of allowed IPs/ports for both outbound and in bound.
  * Stateful- if one direction is allowed, other is not checked.
  * Ex: If an IP is allowed to access the server, then the response is not checked by SG on the way out.
* Network ACL
  * at subnet level
  * can create list of denied AND allowed IPs/ports for both outbound and in bound.
  * Stateless - any request or retrieval involving an instance in an ACL is checked no matter if it was previously checked on the way in.
  * Ex: If an instance connects to google.com and is allowed, the response by google.com to the request will also be checked.
