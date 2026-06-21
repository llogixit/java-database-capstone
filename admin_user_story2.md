Title: As an Admin, I want to log out of the portal to protect system access so that unauthorized users cannot continue using my active session.

Acceptance Criteria
Logout Functionality  
The system must provide a visible "Log Out" option accessible from all admin pages.

Session Termination  
Logging out must immediately invalidate the current session token, preventing further use of the portal without re-authentication.

Redirect Behavior  
After logout, the user must be redirected to the login page with a confirmation message (e.g., "You have been logged out successfully").

Security Enforcement  
Any attempt to access admin pages after logout must require re-entry of valid credentials.

Timeout Handling  
The system must automatically log out inactive sessions after a configurable period of inactivity.

Priority
High — Essential for maintaining system security.

Story Points
3–5 points (lower than login since it’s simpler, but includes session handling and timeout logic).
