# Lab 03 - MFA Enforcement and Account Security in Microsoft 365

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
This lab simulates the process of enforcing multi-factor authentication (MFA) in a Microsoft 365 environment by using Conditional Access.

The purpose of this project is to demonstrate how Conditional Access policies can strengthen account security by requiring additional verification during sign-in.

## Scenario
A small business wants to improve account security for its Microsoft 365 users.

As the IT administrator, I need to review authentication settings, apply MFA-related protections, and verify that the user account is better protected against unauthorized sign-in attempts.

## Objectives
- Review authentication settings for a Microsoft 365 user
- Configure or enforce MFA-related protection
- Understand how stronger authentication improves account security
- Verify the effect of authentication-related security changes
- Practice documentation using a real-world security scenario

## Tools and Services Used
- Microsoft Entra Admin Center
- Microsoft 365 Admin Center
- Authentication methods
- Microsoft Authenticator
- GitHub documentation

## Administrative Workflow
### Step 1: Review the User’s Authentication Methods
- Open Microsoft Entra Admin Center
- Go to **Users** > **All users**
- Select the target user account
- Open **Authentication methods**
- Review the currently registered authentication methods for the user
- Confirm that no usable authentication methods were registered for the user

![Check User Authentication Method](https://raw.githubusercontent.com/ProJensen/Microsoft-365-Lab/refs/heads/main/Lab03-MFA-Enforcement/screenshots/1_Check_User_Authentication_Method.png)

### Step 2: Add a Phone Number Authentication Method
- Select **Add authentication method**
- Choose **Phone number** and enter the user's phone number
- Confirm the phone number was added as an authentication method for the account

This step helps strengthen account security by adding an additional verification method beyond a password-only sign-in.
