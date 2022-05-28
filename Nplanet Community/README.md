# Nplanet Project
https://github.com/lawaty/JS-Libraries

## Overview
This project is a community for engineers (students specifically) where they can publish courses & projects to teach others and earn money.

## My Role
> 1. Project Manager
> 2. Back-End Developer
> 3. Created front-end libraries

## Technologies & Specifications
1. `3-tier` architecture
2. crude PHP backend in `OO structure`
3. `Sqlite DB`
4. `REST API`

5. UI built in `components` structure for reusability & organization
6. `Bootstrap` & `jQuery` UI

7. `Auto-deployment` using git hooks
8. `API is documented` on postman

## Features
### Basic
1. Account Creation and Editing (User can be both student and instructor)
### Courses
2. Course Creation
3. Course Editing
4. Adding Sessions and chapters
5. Browsing Courses
6. Progress tracking from inside the statistics dashboard for each user
### Channels
7. Channels creation
8. Publishing announcements
9. Setting deadlines
10. Managing channel file manager
11. Group Chat
#### Calendar
12. Sync with channels deadlines
13. Custom deadlines for each user
14. Raising notifications and reminders

## Back-end (Technical Keypoints)
1. `Endpoint` Library:
    1. `payload filtering`
    2. `payload validation` based on some regex expectation specified for each endpoint or custom validation functions if regex is not sufficient

2. `DB` Library: respresents an abstraction layer built over PDO that simplifies DB communication by the following:
    1. `accepts arrays` instead of query strings which is more convenient form as request is usually in the form of arrays
    2. performs complex `query formatting` according to the desired action

3. `Authenticator` Library:  
    Automates user credentials validation, token creation, and encrypting/decrypting cyphers using unique secret generated for each entity on the system.  
    Uses multiple encryption approaches that can be easily modified from time to time.

4. `Guardian` library:
    Automates `endpoint routing`, `request validation` and filtering, `API logging`, `failure reporting` if endpoint fails to run and `response formatting` in json that returns error codes, status statements, data for the client if any exists, and encountered problems in detail if exist

## Front-End (Technical Keypoints)
1. `Validator Library`:
    Adding `unregistered html attributes` to input fields to automate validation and provides the following:
    1. `Regex` Validation
    2. Min/Max Lengths
    3. Required and Optional fields
    4. Error Codes

2. Forms Library:
    1. Automates `AJAX communication` and `payload formatting`
    2. Manager the form `UX flow`
    3. Fields Validation using Validator library

3. dependencyManager Library:
    1. manages importing html, css, js files `dynamically and synchronously`
    2. supports `component structuring`
    3. `eliminates importing redundancies`