
# **Hobbits Beauty Parlour Booking Application**

## **Project Overview**

The Hobbits Beauty Parlour Booking Application is a web-based solution designed to modernize the process of booking beauty services. This system enables users to schedule appointments remotely, choose from a variety of services, make secure payments, and receive automated confirmations. By eliminating the need for in-person bookings, the app enhances convenience and efficiency for customers while streamlining operations for beauty service providers.

## **Features**

* Remote Booking: Allows customers to book beauty services from anywhere, anytime.
* Service Availability: Displays real-time availability of beauty professiqonals and services.
* Service Selection: Enables customers to choose their preferred services and professionals based on ratings and expertise.
* Automated Confirmation: Sends digital confirmations with booking details, service provider information, and payment confirmation.
* Flexible Appointment Management: Customers can modify or cancel bookings within specified timeframes.
* Reporting: Generates reports for beauty parlours on bookings, peak hours, and revenue.

## **Problem Statement**

Currently, booking beauty services often requires customers to visit salons or make phone calls, leading to inconvenience and inefficiencies. Manual systems also increase the risk of scheduling conflicts and errors. The Hobbits Beauty Parlour Booking Application aims to:
* Reduce operational inefficiencies and customer wait times.
* Improve accessibility to beauty services by offering an easy-to-use app.
* Automate appointment management and reduce errors.
* Streamline the booking process with real-time availability and service customization.

## **Technology Stack**

* Frontend: HTML, CSS, JavaScript
* Backend: PHP
* Database: MySQL
* Containerization: Dockerfile
* Deployment: Shell scripting for automated deployment

## Installation
### Prerequisites
* PHP (v7.4 or later)
* MySQL database
* Docker (for containerization)
* Web browser (for testing the frontend)
* Xampp Server
* Google Authenticator

### Steps to install
1. Clone the Repository

   Open your terminal or command prompt and run the following command:

   `git clone https://github.com/LosBandidox/FINAL-PROJECT-PLP.git`

2. Download Docker Desktop App and Launch as administrator, make sure the engine has started.

3. Using Windows Powershell as administrator:

   * Run the following commands to check if docker is properly installed:
     
      `docker --version`
     
      `docker-compose --version`
 
   * Navigate to the Project Directory
   
      After cloning, navigate to the project folder

   * Run the following command to start the docker containers:

      `docker compose up -d`
4. Access phpMyAdmin using the the url below to manage the database ie import database (localhost.sql) from db folder into the parlour database 

   `http://localhost:8081`

   * Log in Using:

     Username: php_docker 

     Password: root

   * Import the localhost.sql file
  
5. Access the url/port below to sign up and login into the Booking System

   `http://localhost:8001`

   * Sign up using a valid email
   * Scan the Qr code in the page that follows to get the code using the google authenticator app
   * Log in (Input the code above)

6. Now You can go through the services offered and book your preffered service
7. To access the Admin Panel (To Manage Bookings, Users etc):

   `http://localhost:8001/admin/users.php`
## Beauty_parlour_Management_System

** Open the project using this port**
```bash
php -S localhost:8001
```
** Open mailhog for password reset **
```bash
docker pull mailhog/mailhog
docker run -d -p 8025:8025 -p 1025:1025 mailhog/mailhog
```
