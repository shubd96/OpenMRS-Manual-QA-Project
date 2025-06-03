# Patient registration observations(Day 3)
##Fields Explored
1. Name
2. Gender
3. Birthdate
4. Address
5. Phone Number
6. Relatives

### Observations for Name(field)
- There is no character limit for the Given Name and Family Name fields.
-  Given , Middle and Family Name fields accept special characters and nummbers.
-  Input must be provided sequentially. Without entering the Given Name, other fields remain disabled.
-  Middle name is optional and not required to proceed.
-  User cannot proceed unless the name section is complete.
-  There is an option of unidentified patient where user can proceed without specifying a name.
-  When the Unidentified Patient checkbox is selected, the entire name section becomes disabled.
-  When a similar patient already exists with the same Given and Family Name, a message appears: "A similar patient already exists."

#### Gender
- This field appears only after the name section is completed.
- It displays a drop down menu with two options: Male or Female.
- The user can select only one option.
- Drop down is not keyboard accessible. Options can not be selected using the tab button on keyboard.
- The user cannot proceed to next step of registration without selecting the gender.

#### Birthdate
- This field appears only after the gender section is completed.
- There are three required fields to fill: Day, Month and Year.
- There is no specific sequence required ; all the fields are enabled independently.
- The Day field accepts values between 1 and 31 only; values outside this range are not accepted.
- Both the Day and Year fields does not accept alphabets and special characters as input.
- If alphabets and special characters are entered, an error message appears **Must be a number**.
- The Year field accepts values from 1905 to 2025 only.
- There are options for Estimated Years and Estimated Months in case the exact birthdate is unknown.
- The Estimated Years field accepts values from 0 to 120 only..
- Both the Estimated Years and Estimated Month fields do not accept alphabets and special characters as input, and display the message: **Must be a number**.
- The Estimated Months field accepts values from 0 to 11 only.
- If any value is entered in the Estimated Years or Estimated Months fields, the Day, Month, and Year fields are not disabled, but any input provided in them gets automatically cleared or disappears.
- If all the values are entered in Day, Month and Year, then the Estimated Months and Estimated Years field is automatically disabled.

#### Address
- None of the individual address fields (Address , Address 2, City/Village, State/Province, Country, Postal Code) is mandatory on its own.
- However, leaving all of them blank prevents progression to the next step.
- User needs to provide value for atleast one field.
- All address fields accept alphanumeric values, numbers, and special characters.

#### Phone Number
- Phone Number field is **optional**. User can proceed with registration even if it is blank. 
- The Phone number Field does not accept alphabets and special characters as input except ("+", "-" and "()").
- Input is expected in a **standard phone number format** (e.g., +1-234-567-8901).

#### Relatives
- The **Relatives** section appears during the patient registration process.
- It contains a **dropdown menu** labeled **Relationship Type**, with the following options: Doctor, Sibling, Parent, Aunt/Uncle, Supervisor, Patient, Child, Niece/Nephew, Supervisee.
- Next to the Relationship Type, there's a **Person Name** field which allows typing the name of another person already present in the records.
- **Any registered patient can be linked as a relative**, regardless of whether the selected relationship logically applies (e.g., selecting "Supervisor" and assigning it to a random patient).
- There is no validation to confirm if the selected Person Name actually matches the role chosen in Relationship Type.
- A **plus (+) icon** is present, allowing users to **add multiple relatives**, each with its own Relationship Type and Person Name fields.

> Note: Since there is no backend validation between Relationship Type and Person Name, this may lead to **inaccurate relative associations**. However, this behavior cannot be confirmed as a bug without requirement documents.

### General Behavior – Cancel Button
- After filling out all required details (Name, Gender, Birthdate), if the user clicks the **Cancel** button, they are redirected back to the **Name** section.
- The previously entered details remain intact; the form is not reset.

### Form Submission Behavior
- After clicking the **Submit** button, a message appears: **"Patient record created."**
- To verify the newly created patient record.
- Navigate to the **Find Patient Record** section.
- Type the name of the registered patient in the search bar.
- The patient's details appear in the search results, confirming successful creation.
 
 ### Note on Name Field
- Given and Family Name fields accept numbers and special characters.
- System allows submission with those values.
- No clear requirements available, so not marking it as a bug yet.

### Update on the Patient registration portal (2025-05-23)
- Previously the patient registration form did not show fields for Address, Phone Number or Relatives.
- These fields are now visible during registration.
 

  
 
  






 
