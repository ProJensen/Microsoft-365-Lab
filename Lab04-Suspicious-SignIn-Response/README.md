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
- Review the recent sign-in events for the target user
- Observe multiple failed sign-in attempts within a short time period
- Note that several failures came from **Wembley, Greater London**
- Compare those failed attempts with successful sign-ins from **Toronto, Ontario, Canada**
- Identify the pattern as suspicious and suitable for further response actions

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

## Security Considerations
- Suspicious sign-in activity should be reviewed as quickly as possible
- Password resets and session revocation can help reduce ongoing account risk
- Unusual sign-in prompts may indicate compromised credentials or unauthorized access attempts
- Administrators should verify account protection without unnecessarily disrupting legitimate users

## Common Issues and Troubleshooting

### Issue 1: Sign-in logs do not clearly show suspicious activity
Possible causes:
- The event has not appeared in the logs yet
- The user report is based on an MFA prompt without a successful sign-in
- Additional log review may be needed

### Issue 2: User continues to receive unusual sign-in prompts
Possible causes:
- The account password was previously exposed
- Existing sessions were not fully revoked
- MFA settings were not strengthened after the response

### Issue 3: User cannot sign in after the response actions
Possible causes:
- The password reset was not communicated properly
- Sessions were revoked and the user must sign in again
- Additional authentication steps are required after the security response

## What I Learned
This lab helped me understand that responding to suspicious sign-in activity involves both investigation and containment.

I learned how sign-in logs, password resets, and session revocation can be used together as part of a basic account protection workflow in Microsoft 365.
