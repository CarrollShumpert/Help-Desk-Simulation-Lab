# Help-Desk-Simulation-Lab
Active Directory Help Desk Lab
Overview

This lab simulates common Help Desk and Junior System Administrator tasks in a Windows domain environment. The goal of the lab was to practice real-world IT support workflows including user account management, troubleshooting login issues, and resolving tickets using a help desk ticketing system.

A help desk ticketing system was implemented using osTicket to simulate how IT teams track and resolve user issues in production environments.

All user administration tasks were performed using Active Directory Users and Computers within the domain.

Lab Environment
Infrastructure
Component	Description
Domain Controller	Windows Server running Active Directory
Client Machine	Windows 11 workstation
Domain	corp.local
Ticketing System	osTicket
Virtualization	VirtualBox
Network
Domain Controller provides authentication services
Windows 11 workstation joined to the domain
Help Desk tickets created and resolved through osTicket
Help Desk Ticket Simulations

The following IT support scenarios were simulated within the lab environment using osTicket.

These tasks reflect common Level 1 Help Desk responsibilities.

Ticket 101 – Password Reset
Issue

User reported being unable to log into their workstation due to a forgotten password.

Investigation

The user account was located in Active Directory within the appropriate department Organizational Unit.

Resolution

Password was reset using Active Directory.

User was required to change their password at next login.

Tools Used
Active Directory Users and Computers
Domain Controller administrative tools
Skills Demonstrated
User account management
Identity and access administration
Help desk password reset procedures
Ticket 102 – Account Lockout
Issue

User account became locked after multiple failed login attempts.

Investigation

The user account status was checked in Active Directory.

Resolution

The account was unlocked in the user account properties.

User was then able to log into the workstation successfully.

Tools Used
Active Directory Users and Computers
Skills Demonstrated
Account lockout troubleshooting
Authentication issue resolution
Ticket 103 – New Employee Account Creation
Issue

A new employee required access to company systems.

Investigation

Departmental Organizational Units were reviewed to determine proper account placement.

Resolution

A new domain user account was created and placed in the appropriate Organizational Unit.

User account was configured with:

Username
Temporary password
Required password change at first login
Tools Used
Active Directory Users and Computers
Skills Demonstrated
User provisioning
Identity lifecycle management
Ticket 104 – Desktop Standardization Using Group Policy
Issue

The HR department required a standardized desktop background across all user machines.

Investigation

A Group Policy Object was created and configured to apply the desktop wallpaper.

Resolution

The Group Policy Object was linked to the HR Organizational Unit so it applied only to HR users.

Users within the HR department received the standardized desktop background after policy refresh.

Tools Used
Group Policy Management Console
Skills Demonstrated
Group Policy administration
Organizational Unit management
Centralized workstation configuration
Ticketing System Workflow

A help desk ticketing system was deployed using osTicket to simulate real-world IT support operations.

Typical workflow:

User issue submitted as a support ticket
Ticket reviewed and assigned

Key Skills Practiced

Active Directory Administration
User Account Management
Password Reset and Account Unlock
Group Policy Configuration
Help Desk Ticket Workflow
Troubleshooting Authentication Issues
Issue investigated using administrative tools
Resolution implemented in Active Directory or system configuration
Resolution documented and ticket closed
