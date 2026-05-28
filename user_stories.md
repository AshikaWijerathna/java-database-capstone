# User Story Template

**Title:**
_As a [user role], I want [feature/goal], so that [reason]._

**Acceptance Criteria:**
1. [Criteria 1]
2. [Criteria 2]
3. [Criteria 3]

**Priority:** [High/Medium/Low]
**Story Points:** [Estimated Effort in Points]
**Notes:**
- [Additional information or edge cases]

-Issue 1: Admin Login Functionality

Title: Admin can log into the portal securely

User Story:
As an admin, I want to log into the portal using my username and password so that I can securely manage the platform.

Acceptance Criteria:

Admin can enter username and password
System validates credentials
Successful login redirects admin to dashboard
Invalid credentials display an error message
Password input is masked
Issue 2: Admin Logout Functionality

Title: Admin can log out of the portal

User Story:
As an admin, I want to log out of the portal so that I can protect system access and maintain security.

Acceptance Criteria:

Admin can click a logout button/link
Current session is terminated
Admin is redirected to login page
Restricted pages cannot be accessed after logout without logging in again
Issue 3: Add Doctor Profile

Title: Admin can add doctors to the portal

User Story:
As an admin, I want to add doctor profiles to the portal so that doctors can be managed within the system.

Acceptance Criteria:

Admin can enter doctor details (name, specialization, contact info, etc.)
Required fields are validated
Doctor information is stored successfully in the database
Success message is displayed after creation
Issue 4: Delete Doctor Profile

Title: Admin can delete doctor profiles

User Story:
As an admin, I want to delete a doctor’s profile from the portal so that outdated or inactive profiles can be removed.

Acceptance Criteria:

Admin can select a doctor profile to delete
System asks for deletion confirmation
Doctor profile is removed from the database
Deleted profile no longer appears in the doctor list
Issue 5: View Monthly Appointment Statistics

Title: Admin can run MySQL stored procedure for appointment statistics

User Story:
As an admin, I want to run a stored procedure in MySQL CLI to retrieve the number of appointments per month so that I can track platform usage statistics.

Acceptance Criteria:

Stored procedure exists in the database
Procedure returns monthly appointment counts
Admin can execute the procedure successfully in MySQL CLI
Results display month-wise appointment totals
Errors are handled appropriately if execution fails


Patient----------

Issue 1: View Doctors Without Login

Title: Patient can view doctors without logging in

User Story:
As a patient, I want to view a list of doctors without logging in so that I can explore available doctors before registering.

Acceptance Criteria:

Visitors can access the doctor listing page without authentication
Doctor list displays basic information (name, specialization, availability, etc.)
Users can browse multiple doctor profiles
Restricted actions such as booking require login
Issue 2: Patient Registration

Title: Patient can sign up using email and password

User Story:
As a patient, I want to sign up using my email and password so that I can create an account and book appointments.

Acceptance Criteria:

Patient can enter email and password during registration
Email format is validated
Password meets minimum security requirements
Duplicate email registrations are prevented
Successful registration redirects patient to login or dashboard
Issue 3: Patient Login Functionality

Title: Patient can log into the portal

User Story:
As a patient, I want to log into the portal so that I can manage my bookings and appointments.

Acceptance Criteria:

Patient can enter email and password
System validates credentials
Successful login redirects patient to dashboard
Invalid credentials display an error message
Session is created securely after login
Issue 4: Patient Logout Functionality

Title: Patient can log out of the portal

User Story:
As a patient, I want to log out of the portal so that my account remains secure after use.

Acceptance Criteria:

Patient can click a logout button/link
Current session is terminated
User is redirected to the login or home page
Protected pages cannot be accessed after logout
Issue 5: Book an Appointment

Title: Patient can book an hour-long appointment with a doctor

User Story:
As a patient, I want to log in and book an hour-long appointment with a doctor so that I can receive medical consultation.

Acceptance Criteria:

Only logged-in patients can book appointments
Patient can select a doctor and available time slot
Appointment duration is fixed to one hour
Double-booking is prevented
Confirmation message is displayed after successful booking
Issue 6: View Upcoming Appointments

Title: Patient can view upcoming appointments

User Story:
As a patient, I want to view my upcoming appointments so that I can prepare accordingly.

Acceptance Criteria:

Logged-in patients can access their appointment list
Upcoming appointments display doctor name, date, and time
Past appointments are separated from upcoming appointments
Appointment list updates automatically after booking or cancellation

Doctor-------------

Issue 1: Doctor Login Functionality

Title: Doctor can log into the portal

User Story:
As a doctor, I want to log into the portal so that I can manage my appointments and schedule.

Acceptance Criteria:

Doctor can enter username/email and password
System validates login credentials
Successful login redirects doctor to dashboard
Invalid credentials display an error message
Secure session is created after login
Issue 2: Doctor Logout Functionality

Title: Doctor can log out of the portal

User Story:
As a doctor, I want to log out of the portal so that I can protect my personal and professional data.

Acceptance Criteria:

Doctor can access a logout option
Session is terminated after logout
Doctor is redirected to login or home page
Protected pages cannot be accessed after logout
Issue 3: View Appointment Calendar

Title: Doctor can view appointment calendar

User Story:
As a doctor, I want to view my appointment calendar so that I can stay organized and manage my schedule effectively.

Acceptance Criteria:

Doctor can access a calendar view of appointments
Calendar displays appointment dates and times
Upcoming appointments are clearly visible
Doctor can navigate between days, weeks, or months
Issue 4: Mark Unavailability

Title: Doctor can mark unavailable time slots

User Story:
As a doctor, I want to mark my unavailability so that patients can only book available slots.

Acceptance Criteria:

Doctor can select unavailable dates and times
Unavailable slots are blocked from patient bookings
Doctor can update or remove unavailable periods
Changes are reflected immediately in appointment scheduling
Issue 5: Update Doctor Profile

Title: Doctor can update profile information

User Story:
As a doctor, I want to update my specialization and contact information so that patients always have accurate and up-to-date information.

Acceptance Criteria:

Doctor can edit profile details
Fields include specialization, contact number, email, and bio
Updated information is saved successfully
Changes are visible to patients viewing doctor profiles
Issue 6: View Patient Details for Appointments

Title: Doctor can view patient details for upcoming appointments

User Story:
As a doctor, I want to view patient details for upcoming appointments so that I can be prepared before consultations.

Acceptance Criteria:

Doctor can access patient details from appointment list/calendar
Information includes patient name, appointment time, and relevant details
Only authorized doctors can view patient information
Patient information is displayed securely and accurately

- 
