# AWS Auto-Scaling Web Application

## Project Overview
A self-scaling web application deployed on AWS that automatically handles variable traffic by scaling EC2 instances based on CPU utilization.

## Architecture
- **EC2**: Virtual servers hosting the web application
- **Nginx**: Web server serving the HTML application
- **AMI**: Server snapshot used as template for new instances
- **ALB**: Application Load Balancer distributing traffic
- **Auto Scaling Group**: Manages instances (min:1, max:3)
- **CloudWatch**: Monitors CPU and triggers scaling

## Scaling Policy
- Scale OUT: CPU > 50% → Launch new EC2 instance
- Scale IN: CPU < 50% → Terminate extra instances

## Tech Stack
- AWS EC2, Auto Scaling, ALB, CloudWatch
- Amazon Linux 2023
- Nginx Web Server

## GitHub
https://github.com/AmarPreeth/aws-auto-scaling-webapp
