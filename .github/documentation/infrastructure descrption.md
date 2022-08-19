# Infrastructure

![infrastructure_diagram](./Screenshots/deployment-flow.png)

## AWS

### RDS PostgreSQL Database

- DB-Instance-Name: `udacity-database-1`

- URL: `udacity-database-1.ctlmr6tx0705.us-east-1.rds.amazonaws.com`

- Port: `5432`

- AWS RDS Database Service: Relational database to storing information data

### Elastic Beanstalk

- Env-Name: `Udacityapi1-env`

- URL: `Udacityapi1-env.eba-8zuseyc7.us-east-1.elasticbeanstalk.com`

- AWS Elastic Beanstalk Service: The server runs on Elastic Beanstalk and provide the API. Back-End API build files are stored on S3 Storage Service.

### S3 Buckets

- **Front-End:**

  - ARN: `udacity-ui-bucket`

  - URL: `http://udacity-ui-bucket.s3-website-us-east-1.amazonaws.com `

  - The front-end build is hosted on a S3-Bucket that is publicitly reachable and configured for hosting static websites.

- **Media-Bucket:**

  - ARN: `udacity-media-bucket`

  - The media-bucket stores the media-files that are uploaded. The back-end have a connection to this bucket.

- **Backend-Build-Storage:**

  - ARN: `elasticbeanstalk:us-east-1:821390885875`

  - This S3-Bucket stores the back-end builds. The builds are deployd with eb-cli via pipeline.
