# Iot-Oulu-miniProject1

## What's in this Repo

In this repository, I have pushed all required files to emulate my mini project. This readme file will describe all of the steps needed to bring the project in the running state. You can also contribute to my project by opening a pull request as my project is in its starting phases.

## Project in a Nutshell

Provide a concise overview of your IoT project, its purpose, and any notable features.

## Getting Started

### Requirements

List all the prerequisites or dependencies needed to run your project. Include hardware requirements, software dependencies, and any other external tools or libraries.

### Steps to Get Project Running

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/iot-project-1.git
   cd iot-project-1
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

### Using the Code

Explain how users can interact with or customize the code. Provide examples and usage scenarios.

### Deployment

#### Setting Up EC2 Instance

1. **Launch EC2 Instance:**
   - Log in to the AWS Management Console.
   - Navigate to EC2 and launch a new instance.

2. **Security Groups**
   - Configure security groups to control inbound and outbound traffic to your EC2 instance.
   - Example inbound rule:
     ```
     Type: SSH
     Protocol: TCP
     Port Range: 22
     Source: Your IP Address
     ```

3. **Access Control List (ACL)**
   - Set up ACL rules if needed for additional network-level access control.

### Security Considerations

Provide guidelines on securing your IoT project, such as using secure credentials, encryption, or any other best practices.
