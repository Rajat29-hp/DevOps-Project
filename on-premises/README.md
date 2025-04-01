## DevOps Project: On-Premises Deployment on RHEL 9

---

# Introduction

This project provides an on-premises deployment of a DevOps environment, leveraging MySQL, Memcache, RabbitMQ, Tomcat, and Nginx on Red Hat Enterprise Linux 9 (RHEL 9). It is designed for scalability, high availability, and efficient resource management.

# Prerequisites

Before proceeding, ensure the following: - A fresh installation of RHEL 9 for 5 VM.

- User with sudo privileges.
- Internet access for package installations along with hostfile configuration i.e /etc/hosts.
- Ping should be worked for all the hosts.
- firewalld need to be configured properly.
- Open ports: MySQL (3306), Memcache (11211), RabbitMQ (5672), Tomcat (8080), Nginx (80) on respective VMs.

# Architecture Overview

This setup follows a multi-layer architecture:

- Database Layer → MySQL stores structured data efficiently.
- Caching Layer → Memcache improves performance and reduces database load
- Messaging Layer → RabbitMQ handles asynchronous message communication.
- Application Layer → Tomcat serves Java-based applications.
- Reverse Proxy Layer → Nginx manages incoming requests and load balancing.

![image alt](https://github.com/Rajat29-hp/DevOps-Project/blob/d181ac0e3652c7a595464b509f6a5937f346a999/on-premises/Devops-project-management.jpg)

# Benefits

**Complete Control** – You manage everything yourself, including security and configurations.
**Better Performance** – You can fine-tune the system to run as fast and efficiently as possible.
**Data Privacy** – Your information stays within your own network, ensuring better security.
**Low Latency** – Local servers reduce delays, making applications respond faster.

# Drawbacks

**Requires Regular Maintenance** – You’ll need to handle hardware and software updates manually.
**Expensive Setup** – Buying and maintaining physical servers can be costly. Hard to Scale – Expanding resources takes time compared to cloud-based solutions.
**Complex Management** – Setting up networking, security, and configurations requires expertise.

# Conclusion

This on-premises DevOps stack provides a robust, scalable, and secure environment for enterprise applications. Proper automation, monitoring, and security measures ensure optimal performance and reliability.
