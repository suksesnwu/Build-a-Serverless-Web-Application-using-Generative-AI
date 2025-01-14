# Build-a-Serverless-Web-Application-using-Generative-AI
This project demonstrates how to build a serverless web application using AWS Amplify, Amazon Bedrock, and the Claude 3 Sonnet foundation model. Users can input a list of ingredients, and the application generates recipes based on the input. The app features an HTML-based user interface and a backend to handle AI-generated recipe requests.

## Application Architecture
This application uses AWS Amplify, a GraphQL API built with AWS AppSync, AWS Lambda, and Amazon Bedrock.

<img width="422" alt="build-serverless-app-1 cdd9cf6c11353e0c33edb23e840ca855d878304a" src="https://github.com/user-attachments/assets/4455547b-a414-4fe9-b903-62fac836bcae">

## Tasks Covered:
1. Host a Static Website: Configure AWS Amplify to host the frontend application with continuous deployment.
2. Manage Users: Set up Amplify Auth to enable access to the Amazon Bedrock foundation model.
3. Build a Serverless Backend: Develop a serverless backend to handle web app requests.
4. Call the API from the Static Website: Use Amplify Data to connect the frontend with the backend.
5. Build the Frontend: Link the app’s frontend with the backend.

## Host a Static Website
In this task, I created and deployed a React application to the cloud using AWS Amplify. AWS Amplify provides a Git-based CI/CD workflow, making it easy to build, deploy, and host static websites or single-page applications. Here's a breakdown of the steps I followed:

#### Steps Accomplished:
### 1. Create a New React Application:
- I used Vite to create a React TypeScript application named ai-recipe-generator. The setup involved initializing the project and running the app locally to ensure everything worked before deployment.

#### Commands:
"""
npm create vite@latest ai-recipe-generator -- --template react-ts -y
cd ai-recipe-generator
npm install
npm run dev
"""

### 2. Initialize a GitHub Repository:
- I created a new public repository on GitHub named <b>Build-a-Serverless-Web-Application-using-Generative-AI</b> and pushed the React application to the repository.
- I ran the following commands to initialize Git in the project directory, add the files, commit the changes, and push the code to GitHub.

#### Commands:
"""
git init
git add .
git commit -m "first commit"
git remote add origin git@github.com:<your-username>/ai-recipe-generator.git
git branch -M main
git push -u origin main
"""

### 3. Install Amplify in the Project:

I installed AWS Amplify in the project directory to scaffold the necessary Amplify configurations for future backend and hosting setups.
#### Commands:

"""
npm create amplify@latest -y
git add .
git commit -m 'installing amplify'
git push origin main
"""

### 4. Deploy the App with AWS Amplify:


I connected the ai-recipe-generator GitHub repository to AWS Amplify for continuous deployment.
This involved navigating through the AWS Amplify console, selecting GitHub, authenticating my GitHub account, and choosing the repository and branch for deployment.
After review, I saved the settings, and Amplify automatically deployed the app to a globally available CDN, hosting it under an amplifyapp.com domain.

## Manage Users

## Build a Serverless Backend

## Call the API from the Static Website

## Build the Frontend

## AWS Licence

