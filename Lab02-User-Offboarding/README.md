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
### Step 1: Review the User Account
- Open Microsoft 365 Admin Center
- Go to **Users** > **Active users**
- Select the employee account that will be offboarded
- Review the user's profile information, assigned license, and current status

### Step 2: Block Sign-In
- Open the selected user account
- Review the account settings
- Block sign-in for the departing employee
- Confirm that the account can no longer be used to access Microsoft 365 services

### Step 3: Review and Remove Group Memberships
- Review the user’s current group memberships
- Remove the user from groups that are no longer required
- Confirm that access linked to those groups is no longer needed as part of the offboarding process

### Step 4: Review License Assignment
- Review the Microsoft 365 license assigned to the user
- Remove the license if the organization no longer requires the account to retain active service access
- Confirm that license removal follows the organization’s offboarding process

### Step 5: Verify Offboarding Readiness
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
