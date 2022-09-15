# ecs-service-discovery

This repo demonstrates how to achieve service discovery for internal communication between microservices using AWS ECS Cluster with EC2 launch type.

![alt text](https://github.com/banavalikar/ecs-service-discovery/blob/main/sd.png?raw=true)

## Table of Contents
1. [About this Repo](#About)
2. [How to use the repo](#Examples)
3. [Learning Resources](#Learning)
4. [License](#License)

## About this Repo <a name="About"></a>
When I was looking for examples of service discovery for internal microservices, I was not able to find something that fit my specific need. So I created one myself and it worked well.

## Steps involved <a name="Examples"></a>
1. Git clone the repo 
2. Run npm install 
3. Then build, tag and push the containers for app1 and app2 to ECR (when you create the ECR repos, the commands will be shown). Refer [Learning Resources](#Learning) to know more about how to use ECR.
4. Run CloudFormation templates 1-6 from the IaC folder.
5. Hit endpoints / and /buy-a-unicorn-from-app2 of app1.
6. Delete the Cloudformation stacks after you finish.


## Learning Resources <a name="Learning"></a>
- [Git cheatsheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)
- [AWS ECR](https://docs.aws.amazon.com/AmazonECR/latest/userguide/getting-started-console.html)


# License <a name="License"></a>

This library is licensed under the Apache 2.0 License.

