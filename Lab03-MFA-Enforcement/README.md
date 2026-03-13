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
A small business wants to reduce the risk of unauthorized account access for Microsoft 365 users.

As the IT administrator, I need to create a Conditional Access policy that requires MFA for a test user and verify that the sign-in process is protected by stronger authentication requirements.

## Objectives
- Review Conditional Access availability in Microsoft Entra
- Create a Conditional Access policy for MFA enforcement
- Apply the policy to a test user
- Verify that MFA is required during sign-in
- Practice documentation using a real-world identity security scenario

## Tools and Services Used
- Microsoft Entra Admin Center
- Conditional Access
- Microsoft Entra ID P1
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
