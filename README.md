# Alaaya Technologies — Enterprise IAM Lab

## Project Overview

A hands-on cloud security project demonstrating Identity and Access Management (IAM) using Microsoft Entra ID and Azure Role-Based Access Control (RBAC).

**Objective:** Implement and validate least-privilege access controls in a simulated enterprise environment.

## Environment

- **Organization:** Alaaya Technologies (fictional)
- **Cloud platform:** Microsoft Azure
- **Identity provider:** Microsoft Entra ID
- **Resource group:** `rg-alaaya-dev-lab`
- **Security group:** `SG-Alaaya-Dev-Readers`
- **Test identity:** Alex Developer

## Lab 1 — Group-Based Access Control

### Implementation

1. Created an Azure resource group for development resources.
2. Created a Microsoft Entra security group with assigned membership.
3. Assigned the Azure **Reader** role to the security group at resource-group scope.
4. Created a standard test user and registered MFA.
5. Added the test user to the security group.
6. Signed in as the test user to validate effective permissions.

### Validation Results

| Security Test | Result |
|---|---|
| Test user can access the resource group | Passed |
| Test user inherits Reader access | Passed |
| Test user cannot assign Azure roles | Passed |
| Effective access shows Reader only | Passed |
| Resource deletion authorization | Not directly tested |

### Security Concepts Demonstrated

- Role-Based Access Control (RBAC)
- Principle of least privilege
- Group-based authorization
- Scope inheritance
- Multi-factor authentication (MFA)
- Separation of administrative and standard-user privileges

## Cost Management

- Created a monthly Azure budget of 5 units in the billing currency.
- Configured an actual-spending alert at 80%.
- Verified that no charges were reported during initial setup.

Budget alerts provide notifications but do not automatically prevent spending.

## Next Steps

- Explore custom Azure RBAC roles.
- Investigate Azure RBAC permissions and role inheritance.
- Document permission-validation scenarios.
- Explore Conditional Access and Privileged Identity Management where licensing permits.

## Project Status

**Lab 1: Completed — November 4, 2026**

This project is part of an ongoing hands-on cloud security learning portfolio.
