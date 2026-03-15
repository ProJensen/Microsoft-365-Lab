# Lab 04 - Suspicious Sign-In Response Workflow in Microsoft 365

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
This lab simulates a basic suspicious sign-in response workflow in a Microsoft 365 environment.

The purpose of this project is to demonstrate how an administrator can review sign-in activity, identify potential account risk, and take initial response actions to protect a user account.

## Scenario
A user reports unusual account activity or a suspicious sign-in prompt.

As the IT administrator, I need to review the user’s sign-in activity, check for unusual login details, and take basic response actions to help secure the account.

## Objectives
- Review sign-in activity for a user account
- Identify suspicious or unusual sign-in details
- Take initial response actions to help protect the account
- Understand the importance of account monitoring and rapid response
- Practice documentation using a real-world identity security scenario

## Tools and Services Used
- Microsoft Entra Admin Center
- Sign-in logs
- User account management
- Password reset
- Revoke sessions
- GitHub documentation

## Administrative Workflow
### Step 1: Review the User’s Sign-In Activity
- Open Microsoft Entra Admin Center
- Go to **Users** > select the target user account
- Open **Sign-in logs**
- Review recent sign-in attempts for the user

### Step 2: Identify Suspicious Sign-In Details
- Review the sign-in location, timestamp, application, and status
- Look for unusual activity such as unfamiliar locations, repeated failures, or unexpected sign-in attempts
- Document the suspicious details for further review

### Step 3: Take Initial Response Actions
- Reset the user’s password
- Revoke active sessions for the account
- Review whether MFA should be re-registered or reinforced
- Confirm that the account is placed in a more secure state after the response actions

### Step 4A: Verify Response Actions from the Admin Side
- Review the user account settings after the response actions
- Confirm that the password reset was completed
- Confirm that active sessions were revoked
- Verify that the account has stronger protection after the response workflow

### Step 4B: Verify Access from the User Side
- Attempt to sign in using the user account after the response actions
- Confirm that the previous session is no longer active if applicable
- Verify that the user must use updated credentials or reauthentication steps to access the account

## Expected Outcome
At the end of this lab:
- Recent sign-in activity is reviewed
- Suspicious sign-in details are identified and documented
- Initial response actions are taken to protect the account
- Active sessions are revoked
- The account is placed in a more secure state
