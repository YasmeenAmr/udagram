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
      1- install dependances for udagram-frontend
      2- install dependances for udagram-api
      3- build udagram-frontend
      4- build udagram-api
      5- deploy udagram-frontend
      6- deploy udagram-api
      































