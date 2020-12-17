

Amplify Ecosystem - [Graphic in video](https://www.youtube.com/watch?v=y7AesEGIRYM&feature=youtu.be&t=145)  
Amplify Docs - [Javascript Libraries](https://docs.amplify.aws/lib/q/platform/js)  

# Our Amplify React App

Cooresponding Github repo: [modelearth/amplifyapp](https://github.com/modelearth/amplifyapp/) and resulting website: 
[Code for America AmplifyApp](https://main.d13yspuepcv5kl.amplifyapp.com/)  

**What's cool:**  
Github deployments update website automatically.  
Local edits appear instantly in browser.  

[Amplify Console](https://console.aws.amazon.com/amplify/home) - 
[About the Console](https://docs.aws.amazon.com/amplify/latest/userguide/) - Backend admin users invited within Admin UI  

[AWS Terminology](terminology.html) | 
[Notes on Aurora DB and SageMaker](notes.html)  
<br>

# We used the following setup steps

## Initialize GitHub Repo with React
[Step 1: GitHub with react app](https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/module-one/) 


git remote add origin git@github.com:modelearth/amplifyapp.git

Change to single quotes:

	git commit -m 'initial commit'


## Install Amplify Globally

[Step 2: Add Amplify](https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/module-two/?e=gs2020&p=build-a-react-app-one)

Install the Amplify CLI globally

	npm install -g @aws-amplify/cli

Created amplify-user account and copied secret access key <!-- into core-admin aws/amplify folder -->

	amplify configure
	npx create-react-app amplifyapp
	cd amplifyapp
	npm start

`npm start` will launch a browser. When you make edits in the src folder, the browser will update!

Note that the development build is not optimized.  
To create a production build, use `yarn build` and additional commands to deploy.  

[Go to Amplify Console](https://console.aws.amazon.com/amplify/home)  


## Amplify in a New Directory

Initialize AWS Amplify in a new directory by running.
The [step 2 documentation](https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/module-two/?e=gs2020&p=build-a-react-app-one) shows amplify init including -appid
:

	amplify init


The backend will provide:

	amplify pull --appId YOURAPPID --envName staging

During init, when choosing React Javascript, the prompt provided this default 
Build Command:  (npm run-script build)

	amplify add hosting


Hosting provides two options (selected first):

1. Hosting with Amplify Console (Managed hosting with custom domains, Continuous deployment) 
2. Amazon CloudFront and S3 

Then chose (instead of manual deployment):
Continuous deployment (Git-based deployments) 

## Authentication

GMail account auth to be added.
<!-- 
Perhaps the following could be used for Google (Gmail) auth
maps.g .org account
https://console.developers.google.com/apis/credentials?project=georgia-directory
Project: Georgia Directory 
Credential page
-->

## Add Cognito

Try using and documenting activating Cognito within the Amplify Console first.  
Not sure about second step...

	create-react-app myapp
	yarn add aws-amplify aws-amplify-react
	amplify add auth


[Admin UI for all apps](https://us-east-1.console.aws.amazon.com/amplify/home?region=us-east-1#/)

Go to "Frontend environments" to associate a GitHub repo.  
Only works in Chrome, Brave and Safari advise to delete cookies, even with no prior Safari login.


[AWS Terminology](terminology.html) | 
[Notes on Aurora DB and SageMaker](notes.html)  


## Add a Database

Module 4: [Add a GraphQL API and Database](https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/module-four/?e=gs2020&p=build-a-react-app-intro)  

Compare to these steps:  

[Go here](https://docs.amplify.aws/start/q/integration/js) and click [Get Started](https://sandbox.amplifyapp.com/start#datastore). Choose Blog and rename Blog model to Directory and directoryID.


# Gatsby

https://ealtili.medium.com/deploy-gatsby-with-aws-amplify-console-cli-and-aws-cognito-aws-appsync-a94a48d73465  

Some videos to check out: containers, and machine learning/AI
https://www.youtube.com/watch?v=3a86SFIRvVA

<!--
# Expo for React Native - starter, then detach
https://hackernoon.com/understanding-expo-for-react-native-7bf23054bbcd

	"Many experienced React Native developers do not use Expo. Once you get comfortable with all the steps required to configure your projects yourself and deploy your apps, the benefits of Expo are greatly diminished. Also, if you’re looking for a way to handle over-the-air deployments, Microsoft’s CodePush is still best-in-class.""
-->

