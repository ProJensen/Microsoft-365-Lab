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
### Step 1: Review Conditional Access Availability
- Open Microsoft Entra Admin Center
- Go to **ID Protection** > **Risk-based Conditional Access**
- Access the **Conditional Access** policy page
- Review the dashboard and confirm that the **New policy** option is available

![Conditional Access Page](https://raw.githubusercontent.com/ProJensen/Microsoft-365-Lab/refs/heads/main/Lab03-MFA-Enforcement/screenshots/1_Conditional_Access_Page.png)

### Step 2: Create a Conditional Access Policy
- On the **Conditional Access** policy page, select **New policy**
- Enter the policy name **Require MFA for Test User**
- Under **Assignments** > **Users**, select a single test user account
- Exclude the administrator account to avoid accidental lockout during testing

![Select Test User](https://raw.githubusercontent.com/ProJensen/Microsoft-365-Lab/refs/heads/main/Lab03-MFA-Enforcement/screenshots/2_Select_Test_User.png)

### Step 3: Configure Target Resources and Grant Controls
- Under **Target resources**, select **All resources** (formerly 'All cloud apps')
- Under **Grant**, select **Grant access**
- Enable **Require multifactor authentication**
- Set the policy state to **On**
- Disable **Security Defaults** so that the Conditional Access policy could be enforced
- Create the policy successfully

This step enforces MFA for the selected user when accessing cloud applications.

![Target Resources](https://raw.githubusercontent.com/ProJensen/Microsoft-365-Lab/refs/heads/main/Lab03-MFA-Enforcement/screenshots/3_Target_Resources.png)

![Grant](https://raw.githubusercontent.com/ProJensen/Microsoft-365-Lab/refs/heads/main/Lab03-MFA-Enforcement/screenshots/3_Grant.png)

### Step 4A: Verify Policy Status from the Admin Side
- Return to **Risk-based Conditional Access**
- Review the newly created policy **Require MFA for Test User**
- Confirm that the target test user was included in the policy assignment
- Confirm that **All resources** were selected under **Target resources**
- Confirm that **Require multifactor authentication** was enabled under **Grant**
- Verify that the policy state was set to **On**

This step help confirm that the Conditional Access policy was configured correctly from the administrator side.

### Step 4B: Verify MFA Enforcement from the User Side
- Open **office.com** and attempt to sign in using the test user account
- Enter the user’s work email address and password
- Confirm that the sign-in flow required additional authentication
- Verify that the user was required to complete MFA verification before access was granted

This step helped confirm that MFA enforcement was applied from the end-user perspective.

![Login with Authenticator](https://raw.githubusercontent.com/ProJensen/Microsoft-365-Lab/refs/heads/main/Lab03-MFA-Enforcement/screenshots/4_Login_With_Authenticator.png)

## Expected Outcome
At the end of this lab:
- A Conditional Access policy is created successfully
- MFA is enforced for the selected test user
- The policy is enabled and applied to **All resources**
- The user is required to complete additional authentication during sign-in
- MFA enforcement is verified from both the admin side and the user side

## Security Considerations
- MFA helps reduce the risk of account compromise caused by password-only sign-in
- Conditional Access policies should be tested with a single user or pilot group before broader rollout
- Administrator accounts should be excluded from early testing to prevent accidental lockout
- Disabling Security Defaults should be reviewed carefully before moving to Conditional Access-based enforcement
- MFA enforcement should be implemented in a way that balances security and user access requirements

## Common Issues and Troubleshooting

### Issue 1: Conditional Access policy does not apply
Possible causes:
- The wrong user was selected in the policy assignment
- The policy is still set to **Report-only** instead of **On**
- The target user is excluded from the policy
- Security Defaults are still enabled

### Issue 2: User can still sign in without MFA
Possible causes:
- The Conditional Access policy has not fully propagated yet
- The sign-in attempt did not match the policy scope
- The user accessed a resource that was not affected by the test
- The MFA requirement was not configured correctly in the **Grant** controls

### Issue 3: Conditional Access cannot be enabled
Possible causes:
- Microsoft Entra ID P1 or P2 is not available in the tenant
- Security Defaults are still enabled
- The policy configuration is incomplete

### Issue 4: Administrator account is affected unexpectedly
Possible causes:
- The administrator account was not excluded from the test policy
- The policy scope was too broad during testing
- The policy was enabled before assignments were fully reviewed
