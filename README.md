# Hosting a Full-Stack Application

### using use the provided Udagram app for completing this final project.

For this project i used AWS services and ci-circle to deploy this project 
-aws services used
1-AWS RDS : for database
2-AWS Elastic Beanstalk : as web server
3-AWS 33 : web hosting frontEnd
-CircleCI
For CI/CD automating pipeline


# Project URLs

FrontEnd url : http://david-udagram.s3-website-us-east-1.amazonaws.com/home
BackEnd url : http://udagram-api-dev.eba-iweqw9ms.us-east-1.elasticbeanstalk.com
Database url : udagram.cdmelu9hywjn.us-east-1.rds.amazonaws.com
circle ci url: https://app.circleci.com/pipelines/github/David-Alfons/udagram/17/workflows/5c82ea69-2150-43dc-8598-ebd8355733df

### Environment variables

POSTGRES_USERNAME: database user name
POSTGRES_PASSWORD: database password
POSTGRES_DB: database name
POSTGRES_HOST: database host url
AWS_DEFAULT_REGION: aws region
AWS_PROFILE: aws profile name
AWS_BUCKET: s3 bucket name
AWS_SECRET_ACCESS_KEY: aws secret key
AWS_ACCESS_KEY_ID: aws access ID
URL: BackEnd url
JWT_SECRET: secret-key
DB_PORT: database port
PORT: server port

### to run backEnd script
cd udagram/udagram-api
npm install
npm run dev
npm run build
npm run deploy

### to run frontEnd script
cd udagram/udagram-frontend
npm install
npm run start
npm run build
npm run deploy
