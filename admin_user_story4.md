 As an Admin, I want to delete a doctor’s profile from the portal so that outdated or incorrect accounts are removed and system access remains secure.

Acceptance Criteria
Delete Option  
The portal must provide a clear "Delete" action for each doctor profile in the admin interface.

Confirmation Prompt  
Before deletion, the system must display a confirmation dialog (e.g., "Are you sure you want to delete this doctor’s profile?").

Access Restriction  
Only admins can perform the delete operation; doctors themselves cannot delete their own profiles.

Data Removal  
Once deleted, the doctor’s login credentials and associated permissions must be invalidated immediately.

Audit Logging  
All deletion events must be logged with timestamp, admin ID, and doctor ID for compliance and tracking.

Error Handling  
If deletion fails (e.g., due to system error), the system must notify the admin with a clear error message.

Priority
High — Critical for maintaining accurate and secure system records.

Story Points
3–5 points (depending on complexity of audit logging and data dependencies).
