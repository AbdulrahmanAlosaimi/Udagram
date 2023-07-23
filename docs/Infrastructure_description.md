## Infrastructure Documentation

---
### Infrastructure diagram
![Infrastructure diagram](https://github.com/AbdulrahmanAlosaimi/Udagram/blob/b36fd5a59bc48120369d26f2f43cab67d31a26e7/screenshots/Infrastructure-diagram.png)

---

### Infrastructure description

The infrastructure includes many AWS services that interact with eachother to provide the application, like:

- S3 bucket to host the Front-end
- Elastic Beanstalk environment to host the Back-end API
- RDS instance to host the database

The workflow works as follows:

1. The user access the front-end application using this (s3 bucket) [link](http://deployementprocessprojectbucket.s3-website.us-east-2.amazonaws.com)
2. The application interacts with the (Elastic Beanstalk environment) back-end API, by sending requests
3. The back-end application fetches the needed data from the (RDS instance) database
4. The database provides the necessary data to the back-end which in turn returns it to the front-end to display for the user

---

This project was developed by Abdulrahman Alosaimi as a project for the Full Stack JavaScript Developer Nanodegree
