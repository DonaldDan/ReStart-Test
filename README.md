CloudWatch Logging Setup with CloudWatch Agent
Overview
This project demonstrates how to configure and set up logging using the Amazon CloudWatch Agent on a Linux server. The purpose is to monitor system metrics and logs by pushing data from the server to Amazon CloudWatch. This provides centralized logging and monitoring for system performance, application logs, and custom metrics in real-time.

Steps Involved
Install CloudWatch Agent: Download and install the CloudWatch agent on the Linux instance.

Create IAM Role: Attach an IAM role to the instance with the required permissions (CloudWatchAgentServerPolicy) to allow the agent to push logs and metrics to CloudWatch.

Configure the CloudWatch Agent: Create a configuration file (amazon-cloudwatch-agent.json) specifying what metrics and logs to collect. This includes system metrics like CPU, memory, disk usage, and application logs.

Start and Enable the Agent: Use the command sudo amazon-cloudwatch-agent-ctl to start the agent and ensure it runs at boot.

Verify Logging: Navigate to the CloudWatch console to verify logs and metrics are successfully being pushed from the Linux instance to CloudWatch.

Centralized monitoring and alerting.
Real-time tracking of server health and application performance.
Ability to set custom alarms for automated responses.