# DB-Connection-for-Terraform-Jenkins-proj

This repository contains **database connection code** and configuration for the Flask application to interact with an AWS-hosted database.

## Contents
- `db_connection.py` → Python script for connecting Flask to AWS RDS (PostgreSQL/MySQL).
- `db_config.json` → Database credentials and endpoint (secured via environment variables/secret manager).
- `migrations/` → Database schema or migration scripts.

## Purpose
- Enables secure and persistent data storage for the Flask app.
- Configured to connect to an **AWS RDS instance** provisioned by Terraform.
- Integrated into CI/CD pipelines for environment setup.

## How It Fits in the Project
1. Terraform provisions RDS and security groups.
2. Flask app retrieves DB credentials securely.
3. Jenkins ensures DB connection code is tested and deployed.

---
