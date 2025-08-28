# Java Web App Deployment with AWS CI/CD

Welcome to this project combining Java web app development and AWS CI/CD tools!

<br>

## Table of Contents
- [Introduction](#introduction)
- [Technologies](#technologies)
- [Setup](#setup)
- [Contact](#contact)
- [Conclusion](#conclusion)

<br>

## Introduction
This project is used for an introduction to creating and deploying a Java-based web app using AWS, especially their CI/CD tools.  

The deployment pipeline I'm building around the Java web app in this repository is invisible to the end-user, but makes a big impact by automating the software release processes.  

- I’m doing this project to gain **hands-on DevOps and AWS experience** that I can showcase in my professional portfolio.  
- It also fits into my long-term career goals of becoming a **cloud security and automation consultant**, as it helps me practice real-world workflows that clients would expect.  

<br>

## Technologies
Here’s what I’m using for this project:  

- **Amazon EC2**: I'm developing my web app on Amazon EC2 virtual servers, so that software development and deployment happens entirely on the cloud.  
- **VS Code**: For my IDE, I chose Visual Studio Code. It connects directly to my development EC2 instance, making it easy to edit code and manage files in the cloud.  
- **GitHub**: All my web app code is stored and versioned in this GitHub repository.  
- **[COMING SOON] AWS CodeArtifact**: Once it's rolled out, CodeArtifact will store my artifacts and dependencies, which is great for high availability and speeding up my project's build process.  
- **[COMING SOON] AWS CodeBuild**: Once it's rolled out, CodeBuild will take over my build process. It'll compile the source code, run tests, and produce ready-to-deploy software packages automatically.  
- **[COMING SOON] AWS CodeDeploy**: Once it's rolled out, CodeDeploy will automate my deployment process across EC2 instances.  
- **[COMING SOON] AWS CodePipeline**: Once it's rolled out, CodePipeline will automate the entire process from GitHub to CodeDeploy, integrating build, test, and deployment steps into one efficient workflow.  

**Challenges & Solutions:**  
- *Challenge*: Git didn’t reflect my changes in GitHub initially.  
  *Solution*: I learned to properly stage files (`git add`), commit with a clear message (`git commit -m`), and push to the correct branch (`git push origin main`).  
- *Challenge*: I accidentally created a submodule inside my project.  
  *Solution*: I removed the nested `.git` folder and re-added my files as part of the main repository.  
- *Challenge*: SSH login to EC2 failed due to misplaced keys.  
  *Solution*: I stored my `.pem` file securely in `~/.ssh/` and updated my SSH config so it always connects cleanly.  

<br>

## Setup
To get this project up and running on your local machine, follow these steps:  

1. Clone the repository:  
    ```bash
    git clone https://github.com/yourusername/nextwork-web-project.git
    ```  

2. Navigate to the project directory:  
    ```bash
    cd nextwork-web-project
    ```  

3. Install dependencies:  
    ```bash
    mvn install
    ```  

**Troubleshooting Tips:**  
- If you see *Permission denied (publickey)*, double-check your SSH key setup and file permissions.  
- If GitHub doesn’t update after commits, make sure you are on the **main** branch (`git branch`) and run `git push origin main`.  
- Run `git status` often to verify which files are staged or not.  
- If Nano isn’t available on EC2, install it with `sudo yum install nano -y` or `sudo apt install nano -y` depending on your OS.  

<br>

## Contact
If you have any questions or comments about the NextWork Web Project, please reach out:  

- **Email**: [affiliate.business456@gmail.com](mailto:affiliate.business456@gmail.com)  
- **LinkedIn**: [https://www.linkedin.com/in/louis-moyo](https://www.linkedin.com/in/louis-moyo)  
- **Website/Portfolio**: *(coming soon)*  

![Profile Photo](https://via.placeholder.com/150)  

<br>

## Conclusion
Thank you for exploring this project! I'll continue to build this pipeline and apply my learnings to future projects.  

A big shoutout to **[NextWork](https://learn.nextwork.org/app)** for their project guide and support. [You can get started with this DevOps series project too by clicking here.](https://learn.nextwork.org/projects/aws-devops-vscode?track=high)  

This project has helped me build stronger fundamentals in **Git, AWS, and CI/CD pipelines**. It also marks an important step toward my professional goal of transitioning into a **cloud security and automation consultant role** where I’ll be delivering high-value projects to clients.  
