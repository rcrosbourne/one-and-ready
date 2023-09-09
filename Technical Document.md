## **Technical Document**

### **Project Title**: Employee Transportation Booking Platform

### **Version**: 1.1

### **Date**: September 9, 2023

### **Prepared by**: Rainaldo Crosbourne

### **Approved by**:

### **Document History**

| Version | Date       | Description                             | Author              |
| ------- | ---------- | --------------------------------------- | ------------------- |
| 1.0     | 09/09/2023 | Initial draft of the technical document | Rainaldo Crosbourne |
| 1.1     | 09/09/2023 | Revised based on new inputs             | Rainaldo Crosbourne |

### **Table of Contents**

1. Introduction
2. System Overview
3. Functional Requirements
4. Non-Functional Requirements
5. System Architecture
6. User Roles and Permissions
7. Database Design
8. API Endpoints
9. Frontend Design
10. Project Timeline
11. Conclusion
12. References

### **1. Introduction**

#### **1.1 Background**

This document outlines the technical specifications for a platform that enables employees to reserve seats on buses for home transportation. The system will facilitate the booking process and provide a real-time view for the transport company owner to monitor and manage the bookings.

#### **1.2 Purpose**

To design and implement a secure, reliable, and user-friendly platform to streamline the transportation booking process for employees, and to provide managerial control and real-time insights for transport company owners.

#### **1.3 Scope**

The scope of this project includes the development of a web application with functionalities such as user authentication, seat booking, booking approval by managers, and real-time monitoring and management of seat bookings by transport company owners.

### **2. System Overview**

The system will comprise three primary user roles: Employee, Manager, and Transport Company Owner. It will facilitate seat reservations and approvals, providing a seamless user experience and operational efficiency.

### **3. Functional Requirements**

#### **3.1 User Authentication**

- Users can register and log into the platform using their credentials.
- Secure password storage and retrieval.

#### **3.2 Seat Booking**

- Employees can book seats by specifying the time of transport.
- The booked seat remains in a 'Pending' state until approved by a manager.

#### **3.3 Booking Approval**

- Managers can view, approve, or reject seat bookings.
- Approved bookings change the state from 'Pending' to 'Booked'.

#### **3.4 Booking Management by Transport Owner**

- The transport company owner can confirm to honor or cancel the reservation.
- The transport company owner can view real-time statistics of seat bookings, including the number of seats booked and the respective time slots.

### **4. Non-Functional Requirements**

#### **4.1 Scalability**

- The system should be scalable to accommodate a growing number of users and bookings.

#### **4.2 Security**

- Implement secure data transmission and storage.
- Role-based access control to restrict unauthorized access.

#### **4.3 Performance**

- Optimize for fast response times and smooth user experience.

#### **4.4 Availability**

- Ensure high availability to minimize downtime.

### **5. System Architecture**

#### **5.1 Frontend**

- Technology: ReactJS
- Features: User Authentication, Seat Booking Interface, Manager Approval Interface, Real-time Monitoring and Management Dashboard

#### **5.2 Backend**

- Technology: Laravel
- Features: User Management, Booking Management, Real-time Data Processing

#### **5.3 Database**

- Technology: PostgreSQL
- Features: Storage of User Data, Booking Data, and Transaction Logs

### **6. User Roles and Permissions**

#### **6.1 Employee**

- Can register and log in
- Can book seats with specified time

#### **6.2 Manager**

- Can approve or reject seat bookings

#### **6.3 Transport Company Owner**

- Can confirm to honor or cancel reservations
- Can view real-time statistics of seat bookings

### **7. Database Design**

- Users Table: Stores user details including role (employee/manager/owner), username, hashed password, etc.
- Bookings Table: Stores booking details including user ID, booking time, status (pending/booked), etc.

### **8. API Endpoints**

- `/api/users/register`: User registration
- `/api/users/login`: User login
- `/api/bookings/create`: Create a new booking
- `/api/bookings/approve`: Approve a booking
- `/api/bookings/manage`: Manage booking (confirm/cancel) by transport owner
- `/api/bookings/view`: View booking statistics

### **9. Frontend Design**

- Login Page: Allows users to log in
- Employee Dashboard: Enables employees to book seats
- Manager Dashboard: Enables managers to approve bookings
- Owner Dashboard: Enables the owner to manage and view booking statistics

### **10. Project Timeline**

- Week 1-2: Requirement Gathering and Analysis
- Week 3-4: System Design and Database Setup
- Week 5-8: Backend Development
- Week 9-12: Frontend Development
- Week 13-14: Testing and Deployment

### **11. Conclusion**

This document outlines the technical specifications for the development of an employee transportation booking platform. The system aims to streamline the booking process, providing efficiency and real-time insights for transport company owners.
