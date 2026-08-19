# 🏫 School Management System

A centralized **School Management System** built using **Zoho CRM and Zoho Creator**.

This project manages the complete student lifecycle, from admission enquiries through academic management, attendance, examinations, fees, payments, and parent access.

## 🚀 Project Overview

The solution uses **Zoho CRM as the primary system of record** for school operations and **Zoho Creator as the parent-facing application**.

### Overall Flow

```text
Admission Webform
       ↓
     Leads
       ↓
Admission Process
       ↓
    Students
       ↓
Academic Management
       ↓
┌─────────────┬──────────────┬────────────────┐
│ Attendance  │ Examinations │ Fees & Payments│
└─────────────┴──────────────┴────────────────┘
                       ↓
             Zoho Creator Parent App
```

## 🎯 Objectives

* Manage admission enquiries through a Zoho CRM Webform
* Convert confirmed admissions into student records
* Generate unique Student IDs
* Maintain academic years, classes, sections, subjects, and teachers
* Preserve student academic history
* Record and validate daily attendance
* Manage examinations and student results
* Calculate grades and performance
* Manage student fees and installment payments
* Calculate outstanding fees
* Provide parents with controlled access to their child's information
* Create useful management reports and dashboards
* Implement Deluge automation and business validations
* Integrate Zoho CRM with Zoho Creator

## 🛠️ Technologies

* **Zoho CRM**
* **Zoho Creator**
* **Deluge**
* **Zoho CRM Webforms**
* **Zoho CRM Workflows**
* **Zoho CRM Custom Functions**
* **CRM APIs / Creator Integration**
* **CRM Reports & Dashboards**

## 🧩 Zoho CRM Modules

### Standard Modules

* Leads
* Contacts

### Custom Modules

* Students
* Academic Years
* Classes
* Sections
* Subjects
* Teachers
* Academic History
* Attendance
* Examinations
* Student Results
* Fee Structures
* Student Fees
* Payments

## 🗂️ Data Model

```text
Contacts
   │
   └── Students
          │
          ├── Academic History
          │
          ├── Attendance
          │
          ├── Student Results
          │       ├── Examinations
          │       └── Subjects
          │
          └── Student Fees
                  │
                  └── Payments

Academic Years
   ├── Classes
   │     └── Sections
   │
   ├── Subjects
   │
   └── Examinations
```

## 🔄 Admission Process

```text
Website Admission Form
          ↓
         Lead
          ↓
    Follow-up Process
          ↓
Admission Confirmed
          ↓
     Student Created
          ↓
   Student ID Generated
          ↓
Academic Record Created
```

## ⚙️ Automation

The project uses Zoho CRM workflows and Deluge functions for:

### Student Management

* Automatic Student ID generation
* Admission-to-student processing
* Academic history creation

### Attendance

* Duplicate attendance validation
* Attendance percentage calculation

### Examinations

* Marks validation
* Percentage calculation
* Grade calculation
* Duplicate result prevention

### Fees

* Installment payment processing
* Total amount collected calculation
* Outstanding amount calculation
* Payment status calculation
* Overdue fee identification

## ⭐ Additional Feature

### Low Attendance Alert

An automated low-attendance alert identifies students whose attendance falls below the configured threshold.

This helps school management identify attendance issues early and take appropriate action.

## 👨‍👩‍👧 Parent Application

The Zoho Creator Parent Application allows parents to view information related to their child.

Parents can access:

* Student profile
* Current class and section
* Attendance
* Examination results
* Fee status
* Payment history

Zoho CRM remains the primary source of school data while Zoho Creator provides the parent-facing experience.

## 🔐 Security

The parent application is designed so that a logged-in parent can access only the student record associated with that parent.

```text
Logged-in Parent
       ↓
Parent Mapping
       ↓
CRM Contact
       ↓
Student
       ↓
Authorized Information
```

Parent users should not be able to access another student's information.

## 📊 Reports & Dashboards

The system provides management reports for:

* Admission enquiries
* Admission conversion
* Students by class
* Students by section
* Attendance
* Low-attendance students
* Examination performance
* Class performance
* Fee collection
* Outstanding fees
* Overdue payments

## 🧪 Testing

The implementation is tested for:

* Duplicate Student IDs
* Duplicate attendance records
* Invalid examination marks
* Duplicate examination results
* Multiple fee installments
* Outstanding fee calculation
* Overdue payment identification
* Parent access restrictions
* CRM–Creator data retrieval

## 📸 Project Screenshots

Screenshots of the CRM implementation and Creator Parent Application will be added as the project is completed.

## 📚 Documentation

Detailed project documentation will cover:

* System architecture
* CRM data model
* Module relationships
* Deluge automation
* CRM–Creator integration
* Validation rules
* Testing scenarios

## 👩‍💻 Project Author

**Rohini**

Information Technology Graduate

This project demonstrates practical skills in **Zoho CRM customization, data modelling, Deluge automation, workflow configuration, reporting, and Zoho Creator development**.

