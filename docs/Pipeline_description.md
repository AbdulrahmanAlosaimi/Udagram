## Pipeline Documentation

---

<div align="center">
<h3>Pipeline diagram</h3>
<img src="../screenshots/pipeline-diagram.png">
</div>

---

### Pipeline description

The pipeline was created using [CircleCi](https://circleci.com/), it is connected to the github repository.

The pipeline is triggered upon pushing any local commits to the github repository, the following steps will be executed in the workflow:

- Build: This is the phase the workflow checks that the application can be built before actually deploying it.
  - Environment is set up
  - Depenencies are installed
  - Project is built
- Hold: This is the phase the workflow stops until it receives manual approval
- Deploy: As the name suggests, this is the phase the project will be deployed in
  - Environment is set up
  - aws, eb CLIs are set up
  - Environment variables are configured
  - Dependencies are installed
  - Project is built
  - Front-end and back-end are deployed to an s3 bucket and elastic beanstalk environment respectively

---

This project was developed by Abdulrahman Alosaimi as a project for the Full Stack JavaScript Developer Nanodegree
