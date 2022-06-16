### Summary 
This is a full stack project which is deploied on amazon by using (AWS) services .

### Dependencies
- Node (v14.15.1)
- npm (6.14.8)
- AWS CLI (v2, v1)
- A RDS ( creating database running Postgres)
- A S3 bucket (storing application files and hosting server)
- A IAM (creating user)
- A EB(running server for api)

### Scripts
1-npm run build -> to build www folder
2-npm start -> to start server 
3-npm run deploying -> to deploy application

## Enviromental Variables
POSTGRES_HOST="localhost"
POSTGRES_USERNAME="postgres"
POSTGRES_PASSWORD="postgres"
POSTGRES_DB="udagram"
PORT=8080
PORT_DB=5432
AWS_REGION=""
AWS_PROFILE=""
AWS_BUCKET=""
URL="http://localhost"
JWT_SECRET="secret-should-stay-secret"

## NOTES
1- .env file added into .gitignore file

## Links
- Front-end link :
      http://buc-udagram.s3-website-us-east-1.amazonaws.com

- Back-end link :
      http://udagram-api-dev222.us-east-1.elasticbeanstalk.com/
