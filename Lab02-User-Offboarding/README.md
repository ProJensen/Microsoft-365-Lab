# Lab 02 - User Offboarding and Access Removal

## Table of Contents
- [Overview](#overview)
- [Scenario](#scenario)
- [Objectives](#objectives)
- [Tools and Services Used](#tools-and-services-used)
- [Administrative Workflow](#administrative-workflow)
- [Expected Outcome](#expected-outcome)
- [Security Considerations](#security-considerations)
- [Common Issues and Troubleshooting](#common-issues-and-troubleshooting)
- [What I Learned](#what-i-learned)

## Overview
This lab simulates the offboarding process for an employee leaving an organization in a Microsoft 365 environment.

The purpose of this project is to demonstrate the administrative workflow involved in disabling user access, removing group memberships, managing licensing, and preparing the account for secure offboarding.

## Scenario
An employee is leaving the company and their Microsoft 365 access must be removed.

As the IT administrator, I need to secure the account, remove unnecessary access, and complete the basic offboarding steps to reduce security risk and maintain proper user lifecycle management.

## Objectives
- Review an existing Microsoft 365 user account
- Block sign-in for the departing employee
- Remove the user from assigned groups where appropriate
- Review or remove the assigned Microsoft 365 license
- Understand the importance of secure offboarding and access removal
- Practice documentation using a real-world admin scenario

## Tools and Services Used
- Microsoft 365 Admin Center
- Microsoft Entra Admin Center
- Microsoft 365 user management
- License management
- Group membership management
- GitHub documentation

## Administrative Workflow
### Step 1: Review the User Account and Block Sign-In
- Open Microsoft 365 Admin Center
- Go to **Users** > **Active users**
- Select the employee account that will be offboarded
- Review the user’s profile information, assigned license, and current account status
- Block sign-in for the departing employee
- Confirm that the account can no longer be used to access Microsoft 365 services

![Review User](https://raw.githubusercontent.com/ProJensen/Microsoft-365-Lab/refs/heads/main/Lab02-User-Offboarding/screenshots/1_Review_User.png)

![Block Sign-In](https://raw.githubusercontent.com/ProJensen/Microsoft-365-Lab/refs/heads/main/Lab02-User-Offboarding/screenshots/1_Block_Sign-In.png)

![Blocked](https://raw.githubusercontent.com/ProJensen/Microsoft-365-Lab/refs/heads/main/Lab02-User-Offboarding/screenshots/1_Blocked.png)

### Step 2: Review and Remove Group Memberships
- Review the user’s current group memberships
- Remove the user from groups that are no longer required
- Confirm that access linked to those groups is no longer needed as part of the offboarding process

### Step 3: Review License Assignment
- Review the Microsoft 365 license assigned to the user
- Remove the license if the organization no longer requires the account to retain active service access
- Confirm that license removal follows the organization’s offboarding process

### Step 4: Verify Offboarding Readiness
- Confirm that sign-in is blocked
- Confirm that unnecessary group access has been removed
- Confirm that the license has been reviewed or removed
- Verify that the account is in a secure offboarding state

## Expected Outcome
At the end of this lab:
- The employee account is reviewed for offboarding
- Sign-in access is blocked
- Group memberships are reviewed and updated
- License assignment is reviewed or removed
- The account is placed in a more secure offboarding state

## Security Considerations
- Sign-in should be blocked as early as possible during offboarding
- Access should be removed according to the principle of least privilege
- Group memberships should be reviewed carefully to avoid leaving unnecessary access in place
- License and account actions should follow the organization’s retention and security requirements

## Common Issues and Troubleshooting

### Issue 1: User still appears to have access
Possible causes:
- Sign-in was not fully blocked
- Changes have not propagated yet
- The account is still active in related services

### Issue 2: Group-based access is still present
Possible causes:
- The user was not removed from all relevant groups
- Access is inherited through another group
- Group membership changes have not fully applied yet

### Issue 3: License removal causes unexpected service impact
Possible causes:
- The organization still needs temporary access to mailbox or files
- Offboarding steps were performed in the wrong order
- Retention needs were not reviewed before license removal

## What I Learned
This lab helped me understand that offboarding in Microsoft 365 is an important security process, not just an account cleanup task.

I learned how sign-in blocking, group membership review, and license management work together to reduce risk when an employee leaves the organization. This project also helped me practice documenting an administrative workflow in a structured and professional format.
