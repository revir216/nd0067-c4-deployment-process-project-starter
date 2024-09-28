# Hosting a Full-Stack Application

Link: http://udagram-20240926.s3-website-us-east-1.amazonaws.com

### **You can use you own project completed in previous courses or use the provided Udagram app for completing this final project.**

---

In this project you will learn how to take a newly developed Full-Stack application built for a retailer and deploy it to a cloud service provider so that it is available to customers. You will use the aws console to start and configure the services the application needs such as a database to store product information and a web server allowing the site to be discovered by potential customers. You will modify your package.json scripts and replace hard coded secrets with environment variables in your code.

After the initial setup, you will learn to interact with the services you started on aws and will deploy manually the application a first time to it. As you get more familiar with the services and interact with them through a CLI, you will gradually understand all the moving parts.

You will then register for a free account on CircleCi and connect your Github account to it. Based on the manual steps used to deploy the app, you will write a config.yml file that will make the process reproducible in CircleCi. You will set up the process to be executed automatically based when code is pushed on the main Github branch.

The project will also include writing documentation and runbooks covering the operations of the deployment process. Those runbooks will serve as a way to communicate with future developers and anybody involved in diagnosing outages of the Full-Stack application.

# Udagram

This application is provided to you as an alternative starter project if you do not wish to host your own code done in the previous courses of this nanodegree. The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application.

### Infrastructure

- AWS S3 for storing front-end server

- AWS Elastic Beanstalk for deploying the back-end application.

- AWS RDS for database storage.

- CircleCI for continuous integration and deployment.

- AWS IAM for managing users and permissions.

- Github for version control.

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. 

- npm 6.14.8 (LTS) or more recent.

- AWS CLI v2, v1 can work but was not tested for this project

- AWS RDS for PostgreSQL database. Preferred version is 14.x.

- AWS S3 bucket for hosting front-end files.

```
### Pipeline Process

- Create AWS S3 bucket.
- Create AWS RDS database.
- Test run application locally.
- Configuring CircleCI config file `config.yml` is used to define the pipeline process. It is used to run the tests, and deploy the application to AWS Elastic Beanstalk.
- Create a new repository on Github. Connect the CircleCI project to Github repository.
- Configure environment variables in CircleCI settings.
- Push the code to Github. CircleCI will automatically run the tests and deploy the application to AWS Elastic Beanstalk.
- Check CI pipeline status in CircleCI dashboard. Check log for any errors or warnings.
- The application is now deployed to AWS Elastic Beanstalk. Check again in AWS Elastic Beanstalk to see the deployed application.


## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
