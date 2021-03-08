# aws-ci-cd-deployment
Deploy a Node.js App with CI/CD and AWS.

**Steps:**
1. Initialize a Node.js app, having a server to respond.
2. Push the entire app code to a GitHub repo.
3. Configure AWS ElasticBeanstalk to create a Node environment to deploy the application:
  i. Go to the EBS service, through AWS Console.
  ii. Click on the create application.
  iii. Give an application a name, select Node.js platform.
  iv. Click Create, with Application code as Sample application.
4. Go to CodePipeline service to create a pipeline for this application.
  i. Click on the create pipeline to create a new pipeline.
  ii. Give a name to your pipeline and click next.
  iii. From the source provider select GitHub and connect it to this console.
  iv. Then select the repository you want to deploy and the branch of it.
  v. After configuring these click the next button.
  vi. Then it’ll ask for add build stage (skipped here).
5. Now add where to deploy this code. Before this,confirm that the EBS environment is ready to deploy the application.
6. Now go to CodePipeline console to deploy the application.
7. The app can be tested by clicking on the EBS link or using postman.
8. Now, every time a change is made in the code and pushed it to the repository, this pipeline automatically detects the change and deploys the application again. 

_CodePipeline_
![codepipeline](https://user-images.githubusercontent.com/26769575/110345557-b6f43d00-8054-11eb-81a8-15477c282a2f.JPG)

_Response_
![postman](https://user-images.githubusercontent.com/26769575/110345651-d3907500-8054-11eb-832e-7da6f13025f3.JPG)

