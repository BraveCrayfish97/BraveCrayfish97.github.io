## Day 8 of my Cloud Practitioner Certification
###### Today, I learned about the developer tools offered by AWS along with other data related services.

---

### AWS Developer Tools
* CodeCommit
  * similar to Github
  * hosts secure Git-based repositories
* CodeBuild
  * automates compilation, testing, and production of packages
* CodeDeploy
  * automates software deployment to compute services
* CodePipeline
  * automates the build, test, and deploy phases of the release process
* X-Ray
  * dev tool for debugging

---

### AWS Data-Related Services
* Athena
  * serverless service to run SQL queries on S3 storage
* Elastic Map Reduce (EMR)
  * processes large quantites of data
  * AWS managed service for Hadoop clusters
* Data Pipeline
  * reliably transfers data between compute and storage and also on-prem to cloud
* Glue
  * performs ETL (extract, transform, load) on data usually S3
* Kinesis
  * collects data from real-time streaming data such as sensors
  * 4 types of Kinese Services:
    * Video Streams - securely streams video to AWS for processing
    * Data Streams - pull model - stores data for 1-7 days and allows multiple apps to access that data
    * Data Firehose - push model - sends data to ONE specified app
    * Data Analytics - process and analyze data in the moment instead of sending somewhere to analyze
