
# SQL Server: Roles & Permissions for Claims Management System

This project defines database roles and access controls for a Claims Management System using Microsoft SQL Server.

## Roles Defined

### 🔍 ClaimsAnalyst
- **Purpose**: Read-only access for data analysis and reporting.
- **Permissions**:
  - `SELECT` on: `Claims`, `Policies`, `PolicyTypes`

### 🔧 ClaimsManager
- **Purpose**: Full access for managing claims and updating policy/customer information.
- **Permissions**:
  - `SELECT`, `INSERT`, `UPDATE`, `DELETE` on: `Claims`
  - `SELECT`, `UPDATE` on: `Policies`

## Setup Instructions

1. Create roles:
   ```sql
   CREATE ROLE ClaimsAnalyst;
   CREATE ROLE ClaimsManager;

