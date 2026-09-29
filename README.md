# SMART PRISON — Prison Management System

A role-based web application for managing inmates, staff, visitors, schedules, and administrative operations.

## Overview

Managing a correctional facility involves handling a large amount of information related to inmates, staff, visitors, schedules, and day-to-day administrative activities. When these operations are handled through disconnected records or manual processes, keeping information organized, accessible, and consistent can become challenging.

**SMART PRISON** is a web-based Prison Management System developed to centralize and streamline these operations within a single platform. The goal is to provide authorized staff with a structured environment for managing prison-related information and day-to-day administrative activities while reducing the dependency on scattered or manual processes.

The project is built using **PHP, MySQL, HTML, CSS, and JavaScript**, with the system being developed progressively as new functionality and workflows are introduced.

Beyond building the core management functionality, the project is also being used as a practical way to explore **web application security**. Once the functional foundation is established, the next phase of development will focus on identifying security weaknesses, implementing appropriate security controls, testing the application, and progressively hardening the system.

SMART PRISON is therefore an ongoing project that combines **software development, system design, and practical cybersecurity learning** while continuing to evolve toward a more complete and robust management platform.

### Development Approach

The project is being developed in stages:

**1. System Development**  
Building the core management system, database structure, user roles, workflows, and interface.

**2. Feature Expansion**  
Adding additional operational features such as scheduling, activity tracking, communication, reporting, and other functions as the system develops.

**3. Security Hardening**  
Once the functional foundation is established, the next major phase is to study and implement web application security. This includes identifying weaknesses in the application, applying appropriate security controls, testing the changes, and continuously improving the system.

## Key Features

### Currently Implemented

- Role-based user access
- Inmate management
- Jailor management
- Visitor management
- Visitor request workflow
- Staff scheduling
- Activity history
- Internal communication
- Administrative dashboards

### Planned Features

- Reporting and analytics
- Additional administrative workflows
- Advanced monitoring capabilities
- Additional security controls
- Other features under development

## Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | PHP |
| Database | MySQL |
| Web Server | Apache |
| Development Environment | XAMPP |

## User Roles

The system provides different access levels for **Administrators and prison staff**, allowing each staff member to access the functions relevant to their responsibilities. The system is also designed to be extensible, allowing additional staff roles to be integrated as the project develops.

### Administrator

Responsible for system-wide management and administrative operations.

### Prison Staff

Access operational functions according to their assigned responsibilities.

Additional staff roles, such as **doctors and other medical staff**, may be introduced in future development, with access tailored to their specific responsibilities.

## System Modules

### Login & Authentication

Provides the entry point to the system and controls access to the application through user authentication and role-based access.

![Login Page](SPMS%20SCREENSHOOT/Login_Page.png)

![Login Form](SPMS%20SCREENSHOOT/Enter_Username_Pass.png)

### Role-Based Dashboards

After logging in, users are directed to a dashboard based on their assigned role. The system currently provides separate dashboards for **Administrators** and **Jailor staff**, with each dashboard providing the features and information relevant to that role.

### Administrator Dashboard

The Administrator Dashboard provides centralized access to the main management functions of the SMART PRISON system. It is designed for users responsible for managing the overall system and its operational data.

The dashboard provides an overview of important information and gives administrators direct access to the main management modules. It also includes a **Quick Actions** section that provides shortcuts to frequently used administrative operations.

![Administrator Dashboard](SPMS%20SCREENSHOOT/Admin_Dashboard.png)

![Administrator Dashboard — Additional View](SPMS%20SCREENSHOOT/Admin_2Dashboard.png)

Administrators can access features such as:

- Inmate management
- Staff and Jailor management
- Visitor request management
- Schedule management
- Weekly schedule
- Activity history
- Internal communication
- Quick Actions
- Staff login profile creation
- Other administrative functions

The Administrator Dashboard also provides access to management operations that are not available to regular Jailor staff. For example, administrators can add, edit, and delete records where the corresponding management permissions are required, as well as create staff login profiles and manage the weekly schedule.

### Jailor Dashboard

The Jailor Dashboard provides a more focused interface for regular prison staff. Instead of providing system-wide management controls, it gives Jailor staff access to the information and operational functions required for their responsibilities.

![Jailor Dashboard](SPMS%20SCREENSHOOT/Gate_Jailor_Dashboard.png)

The dashboard provides access to features such as:

- Viewing inmate information
- Viewing visitor-related information
- Viewing the weekly staff schedule
- Viewing activity history
- Internal communication
- Other operational functions available to Jailor staff

Jailor staff can access information through their dashboard but do not have the same administrative management privileges as Administrators. For example, they can view inmate records but cannot edit or delete them, and they can view the weekly schedule created by the Administrator without accessing the schedule management interface.

This separation allows the same system to support different types of users while ensuring that each role is provided with the appropriate functions and level of access.

### Inmate Management

The Inmate Management module provides a centralized interface for maintaining inmate records within the system. Authorized staff can view inmate information and access individual inmate records through the management interface.

Administrators have additional management privileges, allowing them to **add new inmates, edit existing inmate information, and delete inmate records** when required.

Jailor staff can **view inmate records** and access the information needed for their operational responsibilities, but they do not have permission to edit or delete inmate records. This separation of permissions helps ensure that sensitive inmate information can only be modified by authorized administrative users.

The module includes dedicated interfaces for:

**Viewing inmate records**

![Inmate Management](SPMS%20SCREENSHOOT/inmate_management.png)

**Viewing individual inmate details**

![Inmate Details](SPMS%20SCREENSHOOT/View_inamte.png)

**Adding a new inmate**

![Add Inmate — Step 1](SPMS%20SCREENSHOOT/Add_inamte1.png)

![Add Inmate — Step 2](SPMS%20SCREENSHOOT/Add_inamte2.png)

**Editing existing inmate information — Administrator only**

![Edit Inmate Option](SPMS%20SCREENSHOOT/Edit_inmate_button.png)

![Edit Inmate — Step 1](SPMS%20SCREENSHOOT/edit_inmate1.png)

![Edit Inmate — Step 2](SPMS%20SCREENSHOOT/edit_inmate2.png)

**Deleting inmate records — Administrator only**

![Delete Inmate Confirmation](SPMS%20SCREENSHOOT/pop-up_remove_inmate.png)

The following screenshot demonstrates the inmate view available to Jailor staff, where the Edit and Delete options are not available.

![Jailor Inmate View](SPMS%20SCREENSHOOT/Gate_jailor_cannot_delete-or-edit.png)

### Staff Management

The Staff Management module provides administrators with a centralized interface for managing prison staff within the system. Administrators can view staff records, add new staff members, update existing staff information, and remove staff records when required.

Staff access is controlled through role-based permissions, allowing different categories of staff to access only the functions relevant to their responsibilities. The system can also be extended in the future to support additional staff categories, such as doctors and other medical personnel.

The module includes dedicated interfaces for:

**Viewing staff records**

![Staff Management](SPMS%20SCREENSHOOT/jailor_section.png)

**Viewing individual staff details**

![Staff Details](SPMS%20SCREENSHOOT/jailor_details1.png)

![Staff Details — Additional View](SPMS%20SCREENSHOOT/Jailor_Details2.png)

**Adding new staff members**

![Add Staff — Step 1](SPMS%20SCREENSHOOT/add_jailor1.png)

![Add Staff — Step 2](SPMS%20SCREENSHOOT/add_jailor2.png)

**Editing existing staff information**

Staff records can be updated by authorized administrators.

**Deleting staff records — Administrator only**

![Delete Staff Confirmation](SPMS%20SCREENSHOOT/pop_up_remove_jailor.png)

**Quick Actions**

The Administrator Dashboard provides **Quick Actions** for frequently used staff-management functions, including a shortcut for creating new staff login profiles. This allows administrators to quickly create the credentials required for staff members to access the system.

![Create Staff Login Profile](SPMS%20SCREENSHOOT/create_staff_loggin.png)

![Staff Quick Action](SPMS%20SCREENSHOOT/Quick_action%20Jailor.png)

Staff records and system login profiles serve different purposes: staff-management interfaces maintain staff information, while login-profile creation provides the credentials required for authorized staff to access the application.

### Visitor Management

The Visitor Management module provides a structured workflow for handling inmate visitor requests from submission to approval.

The process begins at the **gate**, where gate staff can create a new visitor request by entering the required visitor and inmate information. Once submitted, the request is forwarded to the **Administrator** for review.

The Administrator can review the submitted request and decide whether to **approve or reject** it. This allows visitor requests to be evaluated before they are accepted into the system.

Once the request has been processed, the resulting status is reflected across the system. **Jailor staff can see the relevant changes on their dashboard**, allowing them to stay informed about visitor requests and their current status without having to handle the approval process themselves.

This creates a workflow where each role has a clearly defined responsibility:

- **Gate Staff** — Submit new visitor requests with the required information.
- **Administrator** — Review submitted requests and approve or reject them.
- **Jailor Staff** — View the resulting visitor-request information and status through their dashboard.
- **System** — Keeps the request status updated across the relevant interfaces.

**Gate Staff — New Visitor Request**

![New Visitor Request](SPMS%20SCREENSHOOT/New_visit_request.png)

**Administrator — Visitor Request Review**

![Administrator Visitor Request Review](SPMS%20SCREENSHOOT/New_visit_request_validation_from_admin_dashboard.png)

**Jailor Dashboard — Visitor Request Status**

![Visitor Statistics Updated on Dashboard](SPMS%20SCREENSHOOT/Pending_&_total_visit_of_today_update.png)

**Visitor Request Status**

![Visitor Request Status](SPMS%20SCREENSHOOT/Visit_status_Pending.png)

**Visitor Request History**

![Visitor History](SPMS%20SCREENSHOOT/visit_history.png)

### Schedule Management

The Schedule Management module is designed to organize weekly staff schedules and make them available to authorized staff through the system.

The **schedule management interface is accessible only to Administrators**. Administrators are responsible for creating and managing the weekly schedule, while other authorized prison staff can only view the schedule through the **Weekly Schedule** section available from their dashboard.

The workflow begins with the Administrator selecting the **week for which the schedule needs to be created**. The Administrator then defines the schedule for the staff members across the days of that week, entering the required assignments and activities for each day. Once the schedule is submitted, it is stored in the system and becomes available to authorized staff through the weekly schedule viewing interface.

Staff members do not have access to the schedule-management interface. Instead, they can open the **Weekly Schedule** section from their dashboard and select the relevant week to view the schedule prepared by the Administrator.

This separation ensures that schedule creation and modification remain under administrative control while allowing staff to access the information they need for their daily responsibilities.

The scheduling workflow can be summarized as:

**Administrator → Select Week → Create Weekly Schedule → Save Schedule → Staff Access Weekly Schedule → View Assigned Schedule**

#### Administrator — Schedule Management

The Administrator can:

- Select the week for which a schedule is being created
- Define staff schedules for each day of the week
- Save the completed weekly schedule

![Assigning Staff Schedule](SPMS%20SCREENSHOOT/Assigning_schedule.png)

![Manage Schedule](SPMS%20SCREENSHOOT/Manage_Schedule.png)

#### Administrator & Staff — Schedule Viewing

The Administrator and other authorized staff can:

- View weekly schedules through the staff dashboard
- Select a specific week to view
- Print the displayed weekly schedule if needed

![Access Weekly Schedule](SPMS%20SCREENSHOOT/View_assigned_schedule.png)

![Select Week](SPMS%20SCREENSHOOT/Select_week_dates%20_to_get_the%20actual_schedule.png)

![Weekly Schedule](SPMS%20SCREENSHOOT/Finally_viewed_the_schedule.png)

![Print Weekly Schedule](SPMS%20SCREENSHOOT/Print_schedule.png)

### Activity History & Audit Logging

The Activity History module provides a centralized record of important actions performed within the SMART PRISON system. It allows authorized staff to review what actions have taken place, which user performed them, what part of the system was affected, and when the action occurred.

Whenever an important operation is performed, the system records the activity along with relevant information such as the **username, user role, action performed, affected entity, and timestamp**.

For example, activities such as adding, updating, or deleting an inmate or staff member can be recorded. Visitor requests and schedule-related operations can also be tracked, providing a history of important changes made within the system.

The activity history can be accessed by authorized prison staff through the **Action History** section of the system.

Each activity can provide information about:

- The user who performed the action
- The user's role
- The type of action performed
- The affected part of the system
- The related record or entity
- The time of the activity

![Activity History](SPMS%20SCREENSHOOT/Activity_log.png)

This creates a chronological history of important system operations, making it possible for authorized staff to review changes and understand how the system has been used over time.

### Internal Communication

The Internal Communication module provides a dedicated communication system for authorized prison staff. It allows staff members to communicate with one another directly through the SMART PRISON platform without requiring a separate communication system.

The chat system is available to authorized users according to their assigned roles, allowing communication between staff involved in the day-to-day operation of the facility.

Staff can access the communication section from their dashboard, select the appropriate conversation, and exchange messages with other authorized users. Previous messages remain available within the conversation so that users can follow the ongoing communication.

For example, communication can take place between an Administrator and Jailor staff:

**Administrator sends a message to Jailor staff**

![Message Sent to Jailor](SPMS%20SCREENSHOOT/Message_sent_to_gateJailor.png)

**Jailor staff responds**

![Jailor Response](SPMS%20SCREENSHOOT/Mesage_back_to%20_admin.png)

## Security & Future Development

Security is planned as a major phase of the continued development of SMART PRISON.

The current development has focused primarily on establishing the application's core functionality, database structure, role-based access, and operational workflows. The next phase will focus on evaluating the application from a security perspective and progressively improving its security posture.

The planned security work includes:

- Identifying vulnerabilities within the application
- Reviewing authentication and authorization mechanisms
- Improving input validation and data handling
- Strengthening database security
- Implementing secure password management
- Protecting against common web application vulnerabilities
- Testing the application in an isolated environment
- Applying appropriate security controls
- Continuously reviewing and improving the system

The security phase will also be used as a practical cybersecurity learning process, allowing the application to be tested, weaknesses to be identified, and security improvements to be implemented based on those findings.

Future development may also introduce additional staff roles, operational modules, reporting capabilities, monitoring features, and other functionality as the project evolves.
