# Explanation of the pipeline

For ci/cd I have used jenkins. I have created multistage across all the environments .

We have to select which environment we have to deploy the code. So we have included that in the parameters section.
For dev, prod, uat, there will be different accounts . So in the environment varibles stage we are mentioning the account ids.

Here we are printing the version of the application.

Build tool for nodeJs application is npm. In Install dependencies stage we are using build tool to install all the dependencies required for the application.

Sonarqube is used to test the vulnerabilities of the code.

In sonar-project.properties we give all the inputs required . source files destination project name and project key etc..,

In build stage, we need to infuse the AWS credentials. For that we need to install AWS CREDENTIALS plugin in jenkins.
For every environment we have to build once and we will deploy in different different environments.
In Deploy stage we need to select the environment in jenkins as shown below and start deploying.

Here we need to select the environment which we need to deploy.and click on build. 

__PLUGINS NEED TO INSTALL__

<<<<<<< HEAD
* Aws steps

* Aws credentials

* Pipeline utility steps
=======
Aws steps
Aws credentials
Pipeline utility steps

![1](https://github.com/user-attachments/assets/6a113afe-324e-4cba-b5dd-84e238005169)

![2](https://github.com/user-attachments/assets/e1ef346f-5549-4708-8855-32c6a243e19c)
>>>>>>> b898629f984eec5836da9a46b6aa1354143267f2
