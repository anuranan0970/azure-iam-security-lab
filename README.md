# Azure IAM Security Lab

## Project Overview

This project demonstrates the implementation of Identity and Access Management (IAM) in Azure using Microsoft Entra ID. The objective is to configure secure user access, enforce authentication controls, and apply role-based permissions to cloud resources following enterprise security practices.

---

## Objectives

* Create and manage users in Microsoft Entra ID
* Implement Role-Based Access Control (RBAC)
* Enable Multi-Factor Authentication (MFA)
* Configure Conditional Access policies
* Restrict privileged administrative access
* Monitor identity-related activities

---

## Tools and Services Used

* Microsoft Azure
* Microsoft Entra ID
* Microsoft Defender for Cloud
* Azure Key Vault

---

## Project Architecture

Users are created in Microsoft Entra ID and assigned different roles to control access to Azure resources inside a dedicated Resource Group.

**Access Flow:**
Users → Roles → Resource Group → Secure Access

---

## Implementation Steps

### 1. Resource Group Creation

A resource group named **IAM-Security-Lab** was created to organize all resources used in this project.

### 2. User Creation

Three users were created:

* [securityadmin@testlab.com](mailto:securityadmin@testlab.com)
* [developer@testlab.com](mailto:developer@testlab.com)
* [auditor@testlab.com](mailto:auditor@testlab.com)

### 3. Role Assignment (RBAC)

The following built-in roles were assigned:

* **Security Admin** → Security Reader
* **Developer** → Contributor
* **Auditor** → Reader

### 4. Multi-Factor Authentication (MFA)

MFA was enabled for selected users to strengthen login security.

### 5. Conditional Access Policy

A policy was configured to require MFA for sign-ins from untrusted locations.

### 6. Privileged Access Restriction

Administrative permissions were limited to authorized users only.

### 7. Activity Monitoring

Azure activity logs were reviewed to monitor:

* Login attempts
* Permission changes
* Access failures

---

## Security Features Implemented

* Role-Based Access Control (RBAC)
* Multi-Factor Authentication (MFA)
* Conditional Access
* Least Privilege Principle
* Identity Monitoring

---

## Learning Outcomes

This project helped in understanding:

* Azure identity security fundamentals
* Enterprise IAM design principles
* Practical cloud access governance

---

## Resume Description

Configured Azure IAM using Microsoft Entra ID with RBAC, MFA, and Conditional Access policies for secure enterprise access control.

---

## Future Enhancements

* Integrate Azure Key Vault access restrictions
* Connect logs to Microsoft Sentinel
* Simulate unauthorized login detection

---

## Repository Structure

```bash
Azure-IAM-Security-Lab/
│── screenshots/
│── architecture-diagram/
│── README.md
```
