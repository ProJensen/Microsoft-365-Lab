# Lab 05 - Conditional Access and Device Compliance in Microsoft 365

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
This lab simulates the process of using Conditional Access to restrict access based on device compliance in a Microsoft 365 environment.

The purpose of this project is to demonstrate how administrators can use Conditional Access policies to require a compliant device before allowing access to organizational resources.

## Scenario
A small business wants to improve access control by allowing Microsoft 365 access only from devices that meet organizational compliance requirements.

As the IT administrator, I need to review Conditional Access options, create a policy that requires a compliant device, and document how device-based access control can improve security.

## Objectives
- Review Conditional Access options related to device-based access control
- Create a Conditional Access policy that requires a compliant device
- Apply the policy to a test user
- Understand the relationship between Conditional Access and device compliance
- Practice documentation using a real-world identity and access control scenario

## Tools and Services Used
- Microsoft Entra Admin Center
- Conditional Access
- Microsoft Entra ID P1
- GitHub documentation

## Administrative Workflow
### Step 1: Review Conditional Access Options for Device Compliance
- Open Microsoft Entra Admin Center
- Go to **Conditional Access** > **Policies**
- Review Conditional Access policy options related to device-based access control
- Confirm that the tenant is ready to create another Conditional Access policy for testing

### Step 2: Create a Conditional Access Policy for Device Compliance
- Select **New policy**
- Enter a policy name such as **Require Compliant Device for Test User**
- Under **Assignments** > **Users**, select a single test user account
- Exclude the administrator account to avoid accidental lockout during testing

### Step 3: Configure Device Compliance Grant Controls
- Under **Target resources**, select **All resources**
- Leave additional conditions unconfigured for this basic test
- Under **Grant**, select **Grant access**
- Enable **Require device to be marked as compliant**
- Set the policy state to **On**
- Create and enable the policy
