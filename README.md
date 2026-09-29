# GraySentinel Azure AD & Entra ID Security Deep-Dive

A hands-on Microsoft Entra ID / Azure AD security assessment project focused on identity enumeration, privileged account discovery, service principal analysis, attack-path mapping, password-spray simulation, automation, reporting, and remediation.

## Overview

This project demonstrates a practical Azure AD / Microsoft Entra ID security workflow using:

- ROADrecon
- ROADtools / ROADtx
- AzureHound
- Stormspotter
- Neo4j
- MSOLSpray
- Bash
- Python

The lab focuses on understanding identity relationships, privileged roles, security-enabled groups, service principals, Conditional Access, authentication weaknesses, and attack paths inside an Azure / Entra environment.

## Objectives

The main objectives of this project were to:

- Enumerate Azure AD / Entra ID users
- Identify privileged accounts
- Enumerate security-enabled groups
- Review service principals and application identities
- Collect Azure identity data using AzureHound
- Visualize relationships and attack paths
- Simulate password-spraying in an authorized lab
- Review Conditional Access related weaknesses
- Automate Azure AD security enumeration
- Generate consolidated HTML and JSON reports
- Document remediation recommendations

## Tools Used

| Tool | Purpose |
|---|---|
| ROADrecon | Azure AD / Entra ID enumeration and reconnaissance |
| ROADtx | Azure AD token and authentication-related utilities |
| AzureHound | Collects Azure / Entra identity relationships for graph analysis |
| Stormspotter | Visualizes Azure attack paths and relationships |
| Neo4j | Graph database used by Stormspotter |
| MSOLSpray | Password-spraying testing in authorized environments |
| Bash | Audit automation |
| Python | Consolidated report generation |

## Lab Workflow

```text
Microsoft Entra ID / Azure AD
            |
            v
       ROADrecon
            |
            +--> Users
            +--> Groups
            +--> Roles
            +--> Service Principals
            +--> Conditional Access
            |
            v
       AzureHound
            |
            v
      Identity Graph Data
            |
            v
        Neo4j
            |
            v
      Stormspotter
            |
            v
       Attack Paths

Authorized Password-Spray Lab
            |
            v
        MSOLSpray
            |
            v
Authentication Weakness Review

            |
            v
      Bash Automation
            |
            v
      Python Reporting
            |
            v
   Consolidated HTML Report
