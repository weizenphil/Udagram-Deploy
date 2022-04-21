# Hosting a Full-Stack Application

### **You can use you own project completed in previous courses or use the provided Udagram app for completing this final project.**

---

In this project you will learn how to take a newly developed Full-Stack application built for a retailer and deploy it to a cloud service provider so that it is available to customers. You will use the aws console to start and configure the services the application needs such as a database to store product information and a web server allowing the site to be discovered by potential customers. You will modify your package.json scripts and replace hard coded secrets with environment variables in your code.

After the initial setup, you will learn to interact with the services you started on aws and will deploy manually the application a first time to it. As you get more familiar with the services and interact with them through a CLI, you will gradually understand all the moving parts.

You will then register for a free account on CircleCi and connect your Github account to it. Based on the manual steps used to deploy the app, you will write a config.yml file that will make the process reproducible in CircleCi. You will set up the process to be executed automatically based when code is pushed on the main Github branch.

The project will also include writing documentation and runbooks covering the operations of the deployment process. Those runbooks will serve as a way to communicate with future developers and anybody involved in diagnosing outages of the Full-Stack application.

## Link

The link to the application can be seen [here](http://randomudagram1234.s3-website-us-east-1.amazonaws.com/home).

## Installation

Run `npm install` to download the necessary dependencies.

## Running Udagram locally

You will need to create a `.env` file in `udagram-api` with the following variables set:
- AWS_ACCESS_KEY_ID
- AWS_DEFAULT_REGION
- AWS_SECRET_ACCESS_KEY
- JWT_SECRET
- POSTGRES_DB
- POSTGRES_HOST
- POSTGRES_PASSWORD
- POSTGRES_PORT
- POSTGRES_USERNAME
- PORT 
- URL

Open 2 terminal windows:
1. Navigate to `udagram-api` and run `npm run dev`
2. Navigate to `udagram-frontend` and run `npm run start`

Open `http://localhost:3000` in the browser.

# Circlee CI Link
https://app.circleci.com/pipelines/github/bansalayush25/Udagram-Deploy/24/workflows/45578a1a-e49f-4539-a20d-34ef486a36d7
