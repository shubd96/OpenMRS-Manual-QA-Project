# Find Patient Records Observations

## Fields tested in the search
- Identifier
- Name
- Conditions
- Attachments
- Allergies
- Capture Vitals
- Visit Note
- Admit to inpatient
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

  
  
