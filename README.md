# ContainerizeusingEC2

In this repo, I am learning how a Node.js application can be containerized using ECS (Elastic Container Service) on AWS.

---

## Steps Followed:

1. Initialize an empty Bun app  
   ```bash
   bun init
2. Add Express and type definitions
   bun add express @types/express
3. Write a basic Node.js app in index.ts
4. Write a Dockerfile to containerize the app
5. Build the Docker image
   docker build -t node-app .
6. Test the image locally using Docker
7. Go to ECR (Elastic Container Registry) on AWS and create a new repository
8. Go to IAM, create a user with programmatic access, and connect AWS CLI to your terminal using aws configure
9. Authenticate Docker with ECR and push your image (commands provided in ECR push section)
10. Go to ECS, create a Cluster, define a Task Definition and Service, and configure Auto Scaling Policies