As a Doctor, I want to log out of the portal so that my account and patient data remain secure after I finish managing appointments.

Acceptance Criteria
Logout Option  
The portal must provide a visible "Log Out" button accessible from all doctor pages.

Session Termination  
Logging out must immediately invalidate the doctor’s session token, preventing further access without re-authentication.

Redirect Behavior  
After logout, the doctor must be redirected to the login page with a confirmation message (e.g., "You have been logged out successfully").

Security Enforcement  
Any attempt to access doctor pages after logout must require re-entry of valid credentials.

Timeout Handling  
The system must automatically log out inactive doctor sessions after a configurable period of inactivity.

Priority
High — Essential for protecting doctor accounts and sensitive patient data.

Story Points
3–5 points (simpler than login, but includes session handling and timeout logic).
