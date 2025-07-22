# vProfile — Java Web App on AWS ☁️🚀

A Spring-based Java web application designed for user profile management. Originally built and tested locally, it's now deployed on AWS using services like EC2, S3, Auto Scaling, ACM (HTTPS), and more.

Live App: [https://vprofileapp.kbefkbef.online](https://vprofileapp.kbefkbef.online) *(App will be live for a few hours)*

## 🎥 Demo
Watch a short video demonstrating login to the live application.
https://drive.google.com/file/d/1K2-MDMk2e6qZxb8YwWlzS1T1rFHDcFII/view?usp=sharing


## 🔧 Technologies Used

- **Backend**: Spring MVC, Spring Security, Spring Data JPA  
- **Frontend**: JSP  
- **Build Tool**: Maven  
- **Database**: MySQL 8  
- **Messaging**: RabbitMQ  
- **Caching**: Memcached  
- **App Server**: Apache Tomcat  
- **Search**: Elasticsearch

---

## 🌐 AWS Cloud Architecture

- **Tomcat EC2 Instance**: Hosts the vProfile application
- **Backend EC2 Instances**:
  - MySQL (Database)
  - RabbitMQ (Messaging)
  - Memcached (Caching)
- **S3**: Hosts WAR artifact (uploaded via AWS CLI)
- **ACM**: SSL certificate for HTTPS
- **Route 53 + GoDaddy Domain**: `vprofileapp.kbefkbef.online`
- **Security Groups**:
  - App security group communicates only with backend group
- **Auto Scaling Group**: Configured with policy-based scaling (if required)

 Project Structure
<img width="1838" height="936" alt="Screenshot 2025-07-22 195831" src="https://github.com/user-attachments/assets/e49c479c-2916-469e-91db-281c7a5e1b46" />


