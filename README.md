Countdown Notification Page
A simple web page built with HTML, CSS, JavaScript, and PHP that displays countdown timers and collects email addresses to notify users when the countdown ends.

Features
Countdown Timer: Displays a countdown timer on the web page for any specified date or event.
Email Collection: Allows users to submit their email addresses to be notified when the countdown ends.
Email Notification: Sends an email to all registered users when the countdown reaches zero.
Technologies Used
HTML: For the basic structure of the web page.
CSS: For styling the page and making it visually appealing.
JavaScript: For handling the countdown timer functionality.
PHP: For server-side processing, storing user email addresses, and sending notification emails.
Getting Started
Prerequisites
To run this project, you will need:

A web server with PHP support (e.g., Apache, Nginx)
An SMTP server or a third-party email service for sending emails
Basic knowledge of HTML, CSS, JavaScript, and PHP
Installation
Clone the Repository:

bash

git clone https://github.com/your-username/countdown-notification-page.git
cd countdown-notification-page
Set Up the Project:

Place the project files in the root directory of your web server.
Configure the config.php file with your database and SMTP server details.
Create the Database:

Create a database (e.g., countdown_db).
Import the SQL file (database.sql) to create the necessary tables for storing email addresses.
Run the Application:

Open your web browser and navigate to http://localhost/countdown-notification-page.
Usage
Set Up the Countdown:

Modify the JavaScript code in index.html to set the desired date and time for the countdown.

javascript

const countdownDate = new Date("Dec 31, 2024 23:59:59").getTime();
Collect User Emails:

When users visit the page, they can enter their email addresses to receive a notification once the countdown ends.

Send Notifications:

Once the countdown reaches zero, the PHP script will automatically send an email notification to all registered users.

File Structure
index.html: The main web page containing the countdown timer and email form.
styles.css: The stylesheet for styling the web page.
script.js: JavaScript file for handling the countdown logic.
process.php: PHP script to process email submissions and store them in the database.
notify.php: PHP script to send email notifications when the countdown ends.
config.php: Configuration file for database and SMTP settings.
database.sql: SQL file to create the required database tables.
