# CareShift

CareShift is a care workforce shift management application built with **FlutterFlow** and **Firebase**. The project demonstrates how care workers and managers can manage shifts, client information, care records and operational workflows through a single application.

## Project Purpose

The aim of CareShift is to provide a simple digital workflow for managing care shifts. Workers can view and claim available shifts, access client information, record care activities and complete shifts. Managers can monitor shift activity and access management functions.

## Key Features

### Care Worker
- Secure user login
- View available shifts
- View shift date, start/end time, location, pay rate and status
- Claim available shifts
- View claimed shifts
- View detailed shift information
- Start and complete shifts
- Access client information linked to a shift
- Complete care task checklists
- Add care notes
- Report incidents

### Manager
- Manager dashboard
- Shift overview and status counters
- Manage shifts
- Edit existing shift information
- View and manage clients
- View worker information
- View reported incidents

## Shift Workflow

CareShift supports a shift lifecycle where workers can progress through operational stages:

`Available → Claimed → In Progress → Completed`

Shift status changes are stored in Firebase and reflected throughout the application.

## Care Recording

During a shift, workers can record care activities including:

- Personal Care
- Meal Preparation
- Medication
- Mobility
- Housekeeping
- Care Notes
- Incident Reports

These records are stored in Firebase and associated with the relevant shift and worker.

## Firebase Data Model

The application uses Firebase Authentication and Cloud Firestore.

Main Firestore collections:

### `users`
Stores user information including name, email, phone number and role.

### `shifts`
Stores shift information including title, date, start/end time, location, care home, pay rate, status and assigned worker.

### `clients`
Stores client information including name, date of birth, address, care requirements, care plan, notes and emergency contact information.

### `care_records`
Stores care tasks, care notes and incident information recorded during shifts.

Shift documents are linked to client records using Firestore document references.

## Technology Stack

- FlutterFlow
- Flutter / Dart
- Firebase Authentication
- Cloud Firestore
- GitHub

## Application Structure

The application includes:

- Login
- Worker Home / Available Shifts
- My Shifts
- Shift Details
- Care Record
- Manager Dashboard
- Manage Shifts
- Edit Shift
- Manage Clients
- Client Details
- Manage Workers
- Incident Reports

## Project Status

**Interview MVP completed.**

Core worker and manager workflows have been implemented and tested using FlutterFlow Test Mode with Firebase as the backend.

## Source Code

The application was developed using FlutterFlow. Direct source-code export and GitHub synchronization require a supported FlutterFlow plan, so the generated Flutter source code is not included in this repository.

This repository currently serves as project documentation and a portfolio overview of the implemented application.
