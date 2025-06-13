# Bug Reports – OpenMRS Patient Registration Module

This document contains QA bug reports manually tested and tracked during my OpenMRS project. All bugs were logged using **Jira**. 

---

## Bug ID: BUG-001 – Invalid Input Accepted in Given Name Field

**Test Case ID:** TC_005  
**Module:** Patient Registration  
**Field:** Given Name  
**Jira Ticket:** [OQT-1 (Private Jira)](https://shubhamdas100.atlassian.net/browse/OQT-1?atlOrigin=eyJpIjoiNTU1ZGQ0NmEzOWRmNGMxZjhhOTNhNWMwODU3ZjkzZjIiLCJwIjoiaiJ9)

### Steps to Reproduce:
1. Go to the Patient Registration form.  
2. Enter "John@321" in the **Given Name** field. 
3. Try to proceed or submit the form.

### Expected Result:
Input should not be accepted as it contains special characters and numbers, which are not valid characters for name field.

### Actual Result:
Input is accepted without any error message by the field.

### Status:
Fail

### Notes:
There is no clear requirements available but in general the name field should not accept special characters and numbers as input.

---

## Bug ID: BUG-002 – Family Name Field Accepts Invalid Characters

**Test Case ID:** TC_006  
**Module:** Patient Registration  
**Field:**  Name  
**Jira Ticket:** [OQT-1 (Private Jira](https://shubhamdas100.atlassian.net/browse/OQT-2?atlOrigin=eyJpIjoiMmIzNTA2YzA4NzUzNDVkODhmYzU5MjJkODI4YWUyNDYiLCJwIjoiaiJ9)

### Steps to Reproduce:
1. Go to the Patient Registration form  
2. Enter "Diaz#432" in the Family Name field  
3. Try to proceed or submit the form

### Expected:
Input should not be accepted as it contains special characters and numbers, which are not valid characters for name field.

### Actual:
Input is accepted without any error message by the field.

### Notes:
There is no clear requirements available but in general the name field should not accept special characters and numbers as input.

---
## Bug ID: BUG-003 – Middle Name Field Accepts Invalid Characters

**Test Case ID:** TC_008  
**Module:** Patient Registration  
**Field:** Middle Name  
**Jira Ticket:** [OQT-3 (Private Jira)](https://shubhamdas100.atlassian.net/browse/OQT-3?atlOrigin=eyJpIjoiNjdjMzJhNWQ4MzRkNDAwYmI4ZWFlOGE3ZTk2MjMxNTUiLCJwIjoiaiJ9)

### Steps to Reproduce:
1. Go to the Patient Registration form  
2. Enter "michael%543" in the Middle Name field  
3. Try to proceed or submit the form

### Expected:
Input should not be accepted as it contains special characters and numbers, which are not valid characters for name field.

### Actual:
Input is accepted without any error message from the system.

### Notes:
There is no clear requirements available but in general the name field should not accept special characters and numbers as input.

---
## Bug ID: BUG-004 – Name Fields Do Not Auto-Capitalize

**Test Case ID:** TC_012  
**Module:** Patient Registration  
**Field:** Given Name & Family Name  
**Jira Ticket:** [OQT-4 (Private Jira)](https://shubhamdas100.atlassian.net/browse/OQT-4?atlOrigin=eyJpIjoiNzMxMWIxOTJjMzM4NGNmOTljMGNiMDVhYmI3OTc5ZTkiLCJwIjoiaiJ9)

### Steps to Reproduce:
1. Navigate to "Register a Patient" form. 
2. Enter "john" in the Given Name field.
3. Enter "diaz" in the Family Name field.  
4. Proceed to the next step or review the entered names.

### Expected:
Names should be auto-capitalized as “John” and “Diaz”.

### Actual:
Names are not auto-capitalized and remain in lower case.

### Notes:
While there may be no formal requirement, auto-capitalization enhances user experience and data consistency, especially in medical systems.

---
## Bug ID: BUG-005 – Gender Field Not Accessible via Keyboard

**Test Case ID:** TC_004  
**Module:** Patient Registration  
**Field:** Gender  
**Jira Ticket:** [OQT-5 (Private Jira)](https://shubhamdas100.atlassian.net/browse/OQT-5?atlOrigin=eyJpIjoiYjQzN2UyYmQxNDIxNGFmNDg3ZmEwNzg1MTU3MjhhMDciLCJwIjoiaiJ9)

### Steps to Reproduce:
1. Navigate to the "Register a Patient" form  
2. Press the **Tab** key to move to the **Gender** field  
3. Attempt to select a gender option (Male/Female) using the keyboard

### Expected:
User should be able to select between the two options (Male/Female).

### Actual:
User is not able to select any option and error message : "Required" is displayed. 

### Notes:
Expected behavior based on usability standards

---

## Bug ID: BUG-006 – Address Fields Accept Invalid Characters

**Test Case ID:** TC_005  
**Module:** Patient Registration  
**Field:** Address, City, State, Country, Postal Code  
**Jira Ticket:** [OQT-6 (Private Jira)](https://shubhamdas100.atlassian.net/browse/OQT-6?atlOrigin=eyJpIjoiYzZkOTc0YTMxZmZmNDFkZjliN2ZmYjIwODU1YmZjODMiLCJwIjoiaiJ9)

### Steps to Reproduce:
1. Navigate to the "Register a Patient" form  
2. Enter the following in the respective fields:  
   - Address 2: "Flat #A2" 
   - City: "New-York@123"  
   - State: "CA#1"  
   - Country: "U$A"  
   - Postal Code: "T3A@7Z8"  
3. Click the green forward arrow to proceed

### Expected:
Fields should accept all formats in address 2 section and not in other fields like city, state and postal code.

### Actual:
Field accepts all the formats and User is able to proceed  with the registration process without any error message showing up.

### Notes:
Generally the City, State and Postal code field should not accept special characters as input.


