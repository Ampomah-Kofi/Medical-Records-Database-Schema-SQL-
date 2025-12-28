# Medical Records Database Schema (SQL)

## Overview
This project defines a relational database schema for managing medical records.  
The schema models patients, medical history, procedures, departments, and locations using structured SQL tables.

It demonstrates core database design principles including normalization, primary keys, and relational structure.

## Database Purpose
The database supports:
- Patient demographic storage
- Medical diagnosis tracking
- Medical procedure records
- Department and location management
- Structured querying for healthcare analytics

## Tables Overview

### PATIENTS
Stores patient demographic information.

Columns:
- PATIENT_ID. Primary key  
- FIRST_NAME  
- LAST_NAME  
- SSN  
- BIRTH_DATE  
- SEX  
- ADDRESS  
- DEPT_ID  

### MEDICAL_HISTORY
Stores patient diagnosis records.

Columns:
- MEDICAL_HISTORY_ID. Primary key  
- PATIENT_ID  
- DIAGNOSIS_DATE  
- DIAGNOSIS_CODE  
- MEDICAL_CONDITION  
- DEPT_ID  

### MEDICAL_PROCEDURES
Stores medical procedures performed on patients.

Columns:
- PROCEDURE_ID. Primary key  
- PROCEDURE_NAME  
- PROCEDURE_DATE  
- PATIENT_ID  
- DEPT_ID  

### MEDICAL_DEPARTMENTS
Stores hospital or clinic department information.

Columns:
- DEPT_ID. Primary key  
- DEPT_NAME  
- MANAGER_ID  
- LOCATION_ID  

### MEDICAL_LOCATIONS
Stores department location details.

Composite primary key:
- LOCATION_ID  
- DEPT_ID  

Columns:
- LOCATION_NAME  

## Database Design Features
- Clear separation of entities
- Primary keys defined for all tables
- Composite key used for location mapping
- Support for relational joins across tables
- Scalable structure for analytics and reporting

## SQL Operations Included
- Drop table statements for clean resets
- Create table statements with constraints
- Explicit primary key definitions

## Use Cases
- Patient record management
- Medical history analysis
- Procedure tracking
- Department performance reporting
- Healthcare data analytics

## Technologies Used
- SQL
- Relational database concepts

## How to Use
1. Run the DROP TABLE statements to reset the database
2. Execute the CREATE TABLE statements in order
3. Insert data as required
4. Query tables using SQL joins for analysis

## Skills Demonstrated
- Relational database design
- SQL DDL statements
- Primary and composite keys
- Healthcare data modeling
- Data normalization principles
