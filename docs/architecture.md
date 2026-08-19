# System Architecture

## Overview

The School Management System uses Zoho CRM as the primary system of record and Zoho Creator as the parent-facing application.

## High-Level Flow

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

## Core Principle

Zoho CRM stores and manages the primary school data.

Zoho Creator provides parents with a controlled interface to view information related to their child.

## Main CRM Areas

* Admission Management
* Student Management
* Academic Management
* Attendance Management
* Examination Management
* Fee & Payment Management

## Parent Application

The Zoho Creator application provides access to:

* Student profile
* Current class and section
* Attendance
* Examination results
* Fee status
* Payment history

## Security

Parent access is restricted to the student associated with the authenticated parent.

## Scalability

The system is designed to minimize unnecessary duplicate data and use lookup relationships, workflows, Deluge functions, and controlled CRM–Creator integration.
