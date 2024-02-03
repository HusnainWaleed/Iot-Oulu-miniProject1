# Iot-Oulu-miniProject1

## What's in this Repo

In this repository, I have pushed all required files to emulate my mini project. This readme file will describe all of the steps needed to bring the project in the running state. You can also contribute to my project by opening a pull request as my project is in its starting phases.

## Project in a Nutshell

The IoT Mini Project 1 revolves around the seamless integration of IoT sensors with an IoT cloud, specifically leveraging the capabilities of AWS. The key components and workflow are outlined below:

1. **RIOT-Based Firmware:**
   - The project initiates with the creation of RIOT (Real-Time Operating System for the Internet of Things) based firmware. This firmware acts as the embedded software running on the IoT sensors, facilitating efficient data collection and communication.

2. **Sensor Data Transmission:**
   - The firmware is designed to record sensor data, capturing relevant information from the connected IoT sensors. The primary objective is to create an efficient mechanism for the frequent transmission of this recorded sensor data to the designated IoT cloud.

3. **Requirements for Cloud Communication:**
   - To successfully send data to the IoT cloud (in this case, AWS), several prerequisites must be met:
      - **Driver for the Sensor:** Develop or integrate a sensor driver to enable seamless communication between the sensor and the firmware.
      - **Border Router:** Implement a border router, serving as an intermediary device that facilitates communication between the local IoT network and the broader cloud environment.
      - **Forwarding to the Border Router:** Establish a forwarding mechanism that ensures the collected sensor data is directed towards the border router for subsequent transmission to the IoT cloud.

4. **Cloud Integration (AWS):**
   - Leverage AWS services to receive, process, and store the incoming sensor data. This involves setting up AWS IoT services, configuring necessary security measures, and establishing a communication channel between the IoT devices and the cloud.

5. **Continuous Data Flow:**
   - The project emphasizes the establishment of a continuous and reliable data flow from IoT sensors to the AWS IoT cloud. Achieving this requires robust firmware, sensor drivers, a well-configured border router, and a seamlessly integrated cloud environment.

By orchestrating these elements, the IoT Mini Project 1 aims to provide an illustrative example of connecting IoT sensors to an IoT cloud, with a particular focus on AWS. Through this project, users can gain hands-on experience in creating RIOT-based firmware, managing sensor data, and implementing an end-to-end IoT solution.

## Getting Started
By following these steps you will be able to run or emulate our project.

### Requirements

Before diving into the implementation of the IoT Mini Project 1, ensure that the following requirements are met to guarantee a smooth and successful deployment:

1. **Hardware Requirements:**
   - **IoT Sensors:** Acquire compatible IoT sensors capable of providing the required data for your project. Ensure these sensors are supported by RIOT and have the necessary interfaces for communication.
   - **Border Router:** Set up a dedicated device to act as a border router, facilitating communication between local IoT devices and the broader network, specifically the AWS IoT cloud.

2. **Software Requirements:**
   - **RIOT OS:** Install and configure the RIOT operating system on the IoT sensors. Refer to the [RIOT OS documentation](https://riot-os.org/) for installation guidelines and supported hardware platforms.
   - **Sensor Driver:** Develop or obtain a suitable driver for the IoT sensors, ensuring compatibility with RIOT OS. The driver should enable seamless communication between the firmware and the sensors.
   - **Border Router Software:** Choose or develop software for the border router, ensuring it is capable of forwarding data from the local IoT network to the AWS IoT cloud.

3. **Cloud Platform:**
   - **AWS Account:** Create an AWS account or use an existing one to set up the necessary cloud infrastructure. Ensure the account has appropriate permissions to configure and manage AWS IoT services.
   - **AWS IoT Services:** Familiarize yourself with AWS IoT Core, AWS IoT Device Management, and other relevant services. Configure these services to handle the incoming sensor data securely and efficiently.

4. **Networking:**
   - **Network Configuration:** Ensure proper network configuration to allow communication between IoT devices, the border router, and the AWS IoT cloud. Configure any necessary firewall settings, ports, and protocols for seamless data flow.

5. **Development Environment:**
   - **IDE and Toolchain:** Set up an integrated development environment (IDE) and toolchain compatible with RIOT OS for firmware development. Common tools include GCC, CMake, and a text editor of your choice.
   - **AWS CLI and SDKs:** Install the AWS Command Line Interface (CLI) and any necessary SDKs for your chosen programming language to interact with AWS services programmatically.

6. **Documentation and References:**
   - **RIOT OS Documentation:** Refer to the official RIOT OS documentation for detailed information on supported platforms, installation procedures, and best practices.
   - **AWS Documentation:** Explore the AWS IoT documentation to understand the configuration options, security considerations, and best practices for integrating IoT devices with the AWS cloud.

By fulfilling these requirements, you lay the foundation for a successful implementation of the IoT Mini Project 1, ensuring a well-integrated and functional IoT system.

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
