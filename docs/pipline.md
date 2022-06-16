### circleci version : 
which is the version of platfrom that our application can use.

### orbs:
set of tools that allow us to configure the pipeline
1- node: circleci/node@4.1.0 -> version of node that will use by circleci.
2- aws-cli: circleci/aws-cli@1.3.1 -> version of aws-cli that will use by circleci.
3- eb: circleci/aws-elastic-beanstalk@2.0.1 -> version of elastic beanstalk
that will use by circleci.

### jobs:
set of actions that circleci will use to run pipeline
  setps:
      1- Sign up environment
      2- Preparing environment variables
      3- Install NodeJS 16.13
      4- Install NPM
      5- Checkout code
      6- Install AWS CLI v2
      7- Disable AWS pager if not already configured
      8- Configure AWS access key id
      9- Configure AWS secret access key 
      10- Configure AWS default region
      11- Setting up elastic beanstalk
      12- Front-end install
      13- Back-end install
      14- Front-end build
      15- Back-end build
      16- Back-end deploy
      17- Front-end deploy 

      































