# Day 1: Manual Testing Exploration of OpenMRS
## Modules to be Explored
- Login (Registration Desk)
- Patient Registration
- Find Patient Record
- Active Visits
## Observations
### Login
- Accepts the credentials : Admin(username) and Admin123(password)
- Displays the error message "Invalid username or password" when either the username or password or both fields are left blank.
- Displays the error message "Invalid username or password" when either the username or password or both fields are incorrect.
- Upon clicking the "Can't log in?" link, the system displays the message: "Please contact your System Administrator."
- Password input is masked with dots while typing.
- Password is case sensitive( rejects admin123 as a password).
- Username is not case sensitive(accepts admin as username).
- Password input gets unmasked after clicking the eye button.
- Dashboard appears after successful login.
- Displays the error message "Failed to change your new password" when attempted to change password.

### UI & Functional Behavior
- Username and Password fields contain proper placeholder text.
- Login supports submission using the 'Enter' key.
- "Can't log in?" link is clickable and navigates as expected.
- Login page layout is responsive on different screen sizes.
- URL uses HTTPS (secure protocol).
- After logout, pressing the browser "Back" button redirects to confirm form resubmision (not dashboard).

>  Initial exploratory testing completed for Login functionality.  
>  Ready to begin writing detailed test cases and bug reports from Day 2.

