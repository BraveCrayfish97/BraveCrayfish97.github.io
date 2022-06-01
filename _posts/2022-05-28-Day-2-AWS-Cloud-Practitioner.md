## Day 2 of my Cloud Practitioner Certification
###### Today, I learned about the difference between Physical Servers, VMs, Containers, and Functions. I also learned about Vertical vs Horizontal Scaling.

---

### Physical vs VM vs Container vs Function
* Physical Servers
  * Entire computers used like regular machines such as a laptop
* VM
  * Virtual servers composed of smaller portions of a larger machine
  * Can have multiple VMs on one physical machine
* Container
  * Essentially a VM that doesn't have an OS, just the application and code that supports it such as JDK.
  * Can be created in seconds instead of minutes
* Functions
  *  Serverless computing - Lambda functions
  *  Just provide code and AWS will take care of everything that needs to be done to run it.


---

### Vertical vs Horizontal Scaling
* Vertical Scaling
  * Increasing the power of the existing server
  * Mostly used only with AWS RDS because they are SQL databases and cannot be partitioned across servers, so when 
you run out of storage on the database, you can vertically scale the server it is sitting on to allow for more storage.
  * Not used for scaling EC2 instances because you have to restart the server everytime you want to vertically scale.
  * Ex: adding RAM, CPU, or storage
* Horizontal Scaling
  * Creating more servers and adding them to the LoadBalancer to handle increased traffic.
  * Most popular way to scale applications because more instances can be created in minutes.

