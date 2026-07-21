---
title: "Worklog Week 4"
date: 2026-07-10
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---


### Objectives for Week 4:

* Understand AWS storage services, focusing on Amazon S3.
* Learn how to create an S3 Bucket, upload objects, configure access permissions, and configure Static Website Hosting.
* Understand basic concepts of bucket policy, object key, versioning, and storage class.

### Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | Reference Sources |
| --- | --- | --- | --- | --- |
| Monday | - Study the overview of AWS storage services.<br>- Learn about Amazon S3, S3 Bucket, Object, Object Key, Region, and Storage Class. | 11/05/2026 | 11/05/2026 | https://cloudjourney.awsstudygroup.com/vi/<br>https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html |
| Tuesday | - Learn how to create an S3 Bucket and upload objects.<br>- Learn about Block Public Access, Object Ownership, and object access permissions. | 12/05/2026 | 12/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html |
| Wednesday | - Learn about S3 Static Website Hosting.<br>- Take notes on index document, error document, and bucket website endpoint.<br>- Try configuring a static website with a simple HTML file. | 13/05/2026 | 13/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html |
| Thursday | - Learn about bucket policy and how to grant read access to objects for a static website.<br>- Learn about CORS in S3 and when CORS needs to be configured for a frontend. | 14/05/2026 | 14/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/example-bucket-policies.html<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/cors.html |
| Friday | - Learn about S3 Versioning, lifecycle, and some storage best practices.<br>- Summarize the steps to deploy a static website using S3.<br>- Take notes on common errors when accessing an S3 website. | 15/05/2026 | 15/05/2026 | https://000057.awsstudygroup.com/vi/<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/Versioning.html<br>https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lifecycle-mgmt.html |

### Lab implementation steps for Week 4:

* Open the S3 Console, select Create bucket, and create a globally unique bucket name.
* Choose a suitable Region, for example ap-southeast-1, then configure Object Ownership and Block Public Access according to the lab requirements.
* Upload static website files such as index.html, error.html, CSS, JavaScript, or images.
* Open the bucket Properties tab, enable Static website hosting, and define the index document/error document.
* Create a bucket policy to allow public read access to objects if the lab requires the website to be publicly accessible.
* Check the website endpoint provided by S3 and test it in a browser.
* Enable Bucket Versioning to track object versions when uploading files again.
* Learn about Lifecycle rule to transition or delete old objects when storage optimization is needed.
* Disable public access or delete the bucket after finishing the lab if it is no longer used.

### Results achieved in Week 4:

* Understood how S3 stores data as objects.
* Understood the structure of Bucket, Object, and Object Key.
* Understood the basic steps to enable Static Website Hosting.
* Understood how bucket policy and public access affect website accessibility.
* Understood that S3 can be used as storage for frontend files or uploaded files in the project.


---