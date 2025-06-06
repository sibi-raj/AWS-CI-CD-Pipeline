# Flask App with CI/CD Deployment on AWS

This project is a simple Python Flask web application deployed on AWS using a fully automated CI/CD pipeline.

## 🚀 What It Does

- Deploys a Flask app automatically to **AWS Elastic Beanstalk**
- Uses **GitHub** for source control
- Triggers **AWS CodePipeline** on every commit
- Runs **AWS CodeBuild** to install dependencies and package the app
- Automatically deploys the build to Elastic Beanstalk

## 🛠 Tech Stack

- Python Flask
- GitHub
- AWS CodePipeline
- AWS CodeBuild
- AWS Elastic Beanstalk
- AWS CloudWatch (for logs and health monitoring)

## 📁 Files Included

- `application.py` – Main Flask app file  
- `requirements.txt` – Python dependencies  
- `buildspec.yml` – Instructions for AWS CodeBuild  

## ⚙ How It Works

1. You push code to GitHub.
2. CodePipeline gets triggered.
3. CodeBuild installs dependencies using `buildspec.yml`.
4. The build is deployed to Elastic Beanstalk.
5. CloudWatch and logs help monitor the deployment.

## ✅ Output

After deployment, visiting the app’s URL shows a simple message like:

"Hello,World"
