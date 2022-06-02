## Day 7 of my Cloud Practitioner Certification
###### Today, I learned about the more advanced AWS Networking concepts that are covered in the Cloud Practitioner Certification exam.

---

### More Advanced AWS Networking Topics
* NAT Gateway
  * AWS managed service that has a route to IG, so it is in public subnet
  * private instances put NAT Gateway in their subnet's route table to gain access to the internet, but internet will not be able to access them.
  * NAT Gateway does this by converting the private IP to a public IP and maps each instance to the generated public IP.
* NAT Instance
  *   same thing as NAT Gateway but it runs on a user created EC2 instance
  *   legacy
* VPN Gateway (site to site VPN)
  * 
* AWS Client VPN (user to AWS)
  * private over-the-internet encrypted and cheap method of connecting on-premise to AWS Cloud
* Direct Connect
  * dedicated expensive high-consistent bandwidth and speed method of connecting on-premise to AWS Cloud
  * physical wire is laid between on-premise and AWS datacenter which may require 3rd party such as Verizon.
* Direct Connect Gateway
  * acts a central point to connect on-premise to multiple VPCs using direct connect
* VPC Peering
  * making a physical connection between VPCs to allow for communication among them
  * can only be done if there are no instances with same private IP 
* Transit Gateway
  * acts as a central point to connect VPCs to each other or with on-premise
  * anything connected to it will also be connected with everything else connected to it
* VPC gateway endpoint
  * used when connecting VPC to S3 and DynamoDB
  * connects thru route table 
* VPC interface endpoint
  * used when connecting VPC to all other AWS services
  * connects to a private IP which allows access to given AWS service

