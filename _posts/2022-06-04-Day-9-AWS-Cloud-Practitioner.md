## Day 9 of my Cloud Practitioner Certification
###### Today, I learned about the security related services and the messaging services offered by AWS.
---

### Security Services
* Web Application Firewall (WAF)
  * WAF allows u to create web ACLs which are rules that block common exploits like cross site scripting and SQL injection
* Shield Standard
  * free and does little other than using Cloudfront to reduce # of server hits
* Shield Advanced
  * 3k per month and gives access to AWS people who can help and allows you to scale for attack at no charge for you
* GuardDuty
  * service that constantly monitors your account for suspicious activity and takes automated action against it
* Detective
  * uses machine learning to figure out root cause of suspicious activity
---

### Messaging Services
* Simple Queue Service (SQS)
  * data/requests stored in a "pull" based queue
* Simple Notification Service (SNS)
  * sends "push" based notifs
  * publisher/subscriber model
* EventBridge (CloudWatch Events)
  * acts as if statement for events and collects data off of messages sent thru it
