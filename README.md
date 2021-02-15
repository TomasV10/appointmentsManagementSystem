# appointmentsManagementSystem

# Heroku 

Entry page: https://appointments-manager-system.herokuapp.com/mvc/appointments/reservation

# Stack
PostgreSQL(pgAdmin 4) database, Spring framework, Thymeleaf template engine.

*Please check your port.

# 1Step
Application accesses the database whose name is "appointments_management"
Please create database with that name.

# 2Step
Import database file to DB you have created ("appointments_management") . File are located in project directory: src/main/resources/dbdump

# 3Step

Check application.properties file for the password and run application.

# 4Step

Intro page: http://localhost:8080/mvc/appointments/reservation
This page is for the customers to reservate appointment with the specialist.
When reservation is succesful, customer will see appointment's info with auto generated code, how much time left before the visit and position in line.
At this page customer may cancel appointment if system's calculated available time is unsuitable.

Login Page: http://localhost:8080/login
Login page is created only for specialist. They are created through a database.
After login you will be redirected to the specialist management panel page: http://localhost:8080/mvc/specialist/managementPanel
Specialist can cancel the visit, change it's state to "BEGUN" "END" "NOTSTARTED" - this option is default.
Specialist only see patients who have registered with him.

Appointment info page: http://localhost:8080/mvc/appointments/searchAppointment
This page is for the customer to check his visit information (how much time is left before the visit, position in line and his generated PIN code),
also customer may cancel appointment.



