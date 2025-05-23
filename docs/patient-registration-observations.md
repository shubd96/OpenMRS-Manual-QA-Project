# Patient registration observations(Day 3)
##Fields Explored
1. Name
2. Gender
3. Birthdate

### Observations for Name(field)
- There is no character limit for the Given Name and Family Name fields.
-  Given , Middle and Family Name fields accepts special characters and nummbers.
-  Input must be provided sequentially. Without entering the Given Name, other fields remain disabled.
-  Middle name is optional and not required to proceed.
-  User cannot proceed with further registration steps unless the name section is complete.
-  There is an option of unidentified patient where user can proceed without specifying a name.
-  When the Unidentified Patient checkbox is selected, the entire name section becomes disabled.

#### Gender
- This field appears only after the name section is completed.
- It displays a drop down menu with two options: Male or Female.
- The user can select only one option.
- The user cannot proceed to next step of registration without selecting the gender.

#### Birthdate
- This field appears only after the gender section is completed.
- There are three required fields to fill: Day, Month and Year.
- There is no specific sequence required ; all the fields are enabled independently.
- The Day field accepts values between 1 and 31 only; values outside this range are not accepted.
- Both the Day and Year fields does not accept alphabets and special characters as input.
- If alphabets and special characters are entered, an error message appears**Must be a number**.
- The Year field accepts values from 1905 to 2025 only.
- There are options for Estimated Years and Estimated Months in case the exact birthdate is unknown.
- The Estimated Years field accepts values from 0 to 120 only..
- Both the Estimated Years and Estimated Month fields do not accept alphabets and special characters as input, and display the message: **Must be a number**.
- The Estimated Months field accepts values from 0 to 11 only.
- If any value is entered in the Estimated Years or Estimated Months fields, the Day, Month, and Year fields are not disabled, but any input provided in them gets automatically cleared or disappears.

### General Behavior – Cancel Button

- After filling out all required details (Name, Gender, Birthdate), if the user clicks the **Cancel** button, they are redirected back to the **Name** section.
- The previously entered details remain intact; the form is not reset.

### Form Submission Behavior
- After clicking the **Submit** button, a message appears: **"Patient record created."**
- - To verify the newly created patient record:
  - Navigate to the **Find Patient Record** section.
  - Type the name of the registered patient in the search bar.
  - The patient's details appear in the search results, confirming successful creation.





 
