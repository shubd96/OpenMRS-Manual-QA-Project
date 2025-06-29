# Find Patient Records Observations

## Fields tested in the search
- Identifier
- Name
- Conditions
- Attachments
- Allergies
- Capture Vitals
- Add Past Visit
- Merge visits
- Schedule Appointment
- Request Appointment
- Mark Patient Deceased
- Edit Registration Information
- Delete Patient

 ### Identifier
 - Every patient has a unique identifier.
 - Each identifier is a combination of letters and numbers.
 - Partial input for identfier is accepted. For example: entering just numbers or alphabets returns the related patient's details.
 - The alphabet part in the identifier is case insensitive. For example: "AB" = "ab"
 - Entering an invalid Identifier displays : "No matching records found".
 - Spaces inserted between the numerical input and alphabetical input is acceptable. The system returns the related patient to the entered identifier.
 - However, **spaces inserted within** the individual components (i.e., between digits or between letters) are **not accepted**:
  > The system displays: **"No matching records found"**
 - The system does not accept special characters entered in the space between the alphabetical and numerical inputs.
 - There is no particular defined length for the numerical and alphabetical inputs. For example: **100XHG** and **1001MH**.
 - User cannot edit the patient id, once it is created.
 - Even after saving the updated information, the Patient ID remains unchanged.

### Name
- Name section is case insensitive. For example: The system will accept both **John Diaz** and **john diaz** as input and display the desired result.
- The required patient details can be found by entering only the family name as well. For example : Entering **diaz** in the name field will display the name **John Diaz**.
- Entering wrong name into the field shows the result: **No matching records found**. For example: abcd.
- Entering partial names for both given name and family name returns the expected patient record. For example: **Jo Di** will display **john diaz** in the list.
- If the user enters only a single letter in the ID or Name section, no data is generated.
- The system does not require full name input; partial names are enough to retrieve results.
- Names can be retrieved by entering only the numbers or alphabets as well. For example: entering **hvl** returns **john diaz** as a result.
- User can change the name after it is created by clicking on edit button in the patient details summary page.

### Conditions
-Clicking on a patient’s name redirects the user to a new page displaying multiple editable sections such as Conditions, Attachments, Allergies, and Appointments.
- The Edit button beside the Conditions section opens a new page showing patient details entered during registration. However, the Patient ID is non-editable.
- A yellow clickable box is available on this page, allowing the user to add notes about the patient.
- **ACTIVE** and **INACTIVE** are the two conditions available with the option of adding a new condition in each case.
- While adding a new condition, typing a partial word shows relevant options from the dropdown list.
- If the desired condition is not listed in the dropdown, users can manually enter it using inverted commas (e.g., "RareCondition").
-  The **Onset Date** can not be a future date. It is already set to the current date.
-  For **INACTIVE** conditions, an additional End Date field appears, which also must not be in the future.

 ### Attachments
- The attachment field is not functional unless the patient has an active visit.
- The attachment field becomes functional after the patient is added to either to an inpatient ward or an outpatient ward.
- This field displays the patient registration details along with the active visit date, time, and patient type.
- The user can add an additional note about the patient by clicking on the yellow box.
- There is an option to upload a file from the computer via the file field. The user can also provide a brief description of the uploaded file using the caption field.
- The user can capture a file directly by clicking on the camera icon located below the caption field.
- The user can clear all input fields at once by clicking the “Clear Form” button.

### Allergies
- The user can add allergens that the patient is allergic to, categorized into three types: Drug, Food, or Other.
- Only one allergen can be selected per type. For example, in the Drug section, the user can choose only one drug at a time.
- Multiple reactions can be selected for the chosen allergen(s).
-The severity of the patient's reaction to the selected allergen can be chosen from three options: Mild, Moderate, or Severe.
- Selecting an allergen is mandatory to save the allergy record; other fields like Reactions, Severity, and Comments are optional.
- The Save button remains disabled until at least one allergen is selected.
- If the allergen the user is searching for is not available in the dropdown, an Other option is provided, allowing the user to enter an allergen not listed.
- A similar Other option is available for Reactions, but filling in the corresponding field is optional to save the allergy.
- A Comments section is provided for any additional description or notes about the allergy.

### Capture Vitals
- Atleast one observation is required to save the vitals.
- Inputs in **Height** and **Weight** are mandatory to calculate **BMI**.
- The unit of measurement for height and weight is **cm** and **kg** respectively.
- The Height field accepts input in the range of 10 cm to 272 cm.
- The Weight field accepts input in the range of 0 kg to 250 kg.
- The Height and Weight fields accept decimal values as input.
- Calculated **BMI** is accurate based on the standard formula.
- The unit of measurement for **Temperature** is Celsius (°C) with an input range between 25°C to 43°C.
- The unit of measurement for **Pulse** is per minute (/min) with an input range between 0/min to 230/min.
- The unit of measurement for **Respiratory rate** is per minute(/min) with an input range between 0/min to 99/min.
- The input range for **Blood Pressure** is (0 to 250)/(0 to 150).
- Unit of measurement for **Arterial blood oxygen saturation (pulse oximeter)** is percentage(%) with an input range of 0 % to 100 %.
- **Arterial blood oxygen saturation (pulse oximeter)** , **Pulse** , **Respiratory rate** and **Blood Pressure** only accepts whole numbers as input.

### Add Past Visit
- This function allows the user to add details about the past visit of the patient.
- If the past visit date is conflicting with any other visits in the system, the system will generate a warning.
- The user can add attachments to the past visit date.
- The system generates a warning "Attention! Attachments will be uploaded to a past visit.".
- System shows a future date in the calendar to add past visit which is not technically right.
- User can not capture vitals or diagnoses for past visit.

### Merge Visits
- This function allows the user to merge multiple visits of the same patient.
- In real life, this feature can allow the doctor to analyze any significant changes in the patient's vitals and health.
- User can still add attachments if required.
- After merging the visits user can see all the details about the patient such as vitals and date/ time of admission.
