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
- Go to **Protection** > **Conditional Access**
- Confirm that Conditional Access is available in the tenant after enabling the Microsoft Entra ID P1 trial
- Review the Conditional Access dashboard before creating a new policy

This step helps confirm that the environment is ready for MFA enforcement by using Conditional Access.
