As a Patient, I want to log out of the portal so that my account remains secure and no unauthorized person can access my bookings after I leave the session.

Acceptance Criteria
Logout Option  
The portal must provide a visible "Log Out" button accessible from all patient pages.

Session Termination  
Logging out must immediately invalidate the patient’s session token, preventing further access without re-authentication.

Redirect Behavior  
After logout, the patient must be redirected to the login page with a confirmation message (e.g., "You have been logged out successfully").

Security Enforcement  
Any attempt to access patient pages after logout must require re-entry of valid credentials.

Timeout Handling  
The system must automatically log out inactive patient sessions after a configurable period of inactivity.

Priority
High — Essential for protecting patient accounts and sensitive booking data.

Story Points
3–5 points (simpler than login, but includes session handling and timeout logic).
