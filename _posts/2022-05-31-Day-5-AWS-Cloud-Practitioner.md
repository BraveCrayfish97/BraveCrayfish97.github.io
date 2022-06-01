## Day 5 of my Cloud Practitioner Certification
###### Today, I learned about the main components of the AWS global infrastructure, the compute services offered, and the different EC2 Instance Types.

---

### AWS Global Infrastructure
* Regions
  * Cluster of AZs with datacenters where you can run services
  * Scattered across the world
* Availability Zones
  * multiple AZs per Region
  * multiple datacenters per AZ
  * each AZ has its own independent power, security, network connections, etc.
* Edge Locations
  * datacenters located closest to users
  * spread across world usually in big cities - provides least latency to users
  * used by CloudFront to cache copies of content to provide quicker access
  * Ex: neighbor makes same request that you are made 5 mins ago, neighbor request will be fullfilled by edgelocation because the response is stored in its cache. 

---

### Compute Services
* EC2
  * Infrastructure as a Service (IAAS)
  * Has full flexibility and control over OS and other configurations
* Lambda
  * Function
  * Allows user to write code onto it
  * Code executes only for max 15 minutes, so cannot run websites on it
* Lightsail
  * simpler alternative to EC2
  * Infrastructure as a Service (IAAS)
  * used by people inexperienced in the cloud
* Elastic Beanstalk
  * Platform as a Service (PAAS)
  * User has no control over OS 
  * Used when you simply want to deploy an application

---

### EC2 Instance Types
* On-Demand
  * Pay-as-you-use model
* Spot Instances
  * Bidding for pay
  * cheapest
  * can be taken away with very little notice due to higher bid
  * use for applications that your fine with going down
* Reserved Instances
  * Reserve server for minimum 6months or 1 year
  * 70 percent discount if you pay up front
* Dedicated Instances
  * Buying entire machine
  * used for sensitive applications and applications that have licenses tied to the machine, so need to make sure when VM stops and comes back up, it is still on same machine.
* Dedicated Hosts
  * VMs created on dedicated instances
  * can be created on any on of your dedicated instances
