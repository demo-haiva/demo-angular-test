### SCRUM-10: Navigating via secondary menu item routes correctly
**Test Case Title:** Secondary Menu Navigation – Route and Selection Validation
- Preconditions:
  - User is authenticated and logged in
  - Secondary menu is visible
- Test Steps:
  1. Locate a secondary menu item labeled "<title>"
  2. Click the "<title>" menu item
- Expected Result:
  - The router navigates to "<url>"
  - The item "<title>" has the "selected" active class

---

### SCRUM-9: Navigating via primary menu item routes correctly and sets active state
**Test Case Title:** Primary Menu Navigation – Route, Active State, and Mobile Behavior
- Preconditions:
  - User is authenticated and logged in
  - Primary menu is visible
- Test Steps:
  1. Locate a primary menu item labeled "<title>" with icon "<icon>"
  2. Click the "<title>" menu item
- Expected Result:
  - The router navigates to "<url>"
  - The menu item "<title>" has the "selected" active class
  - All other menu items do not have the "selected" class
  - On mobile, the menu closes after navigation and focus moves to the main page heading

---

### SCRUM-8: Switching between breakpoints recalculates the layout
**Test Case Title:** Layout Recalculation on Breakpoint Change
- Preconditions:
  - Application is open on a large screen (≥ lg breakpoint)
- Test Steps:
  1. Shrink viewport below the lg breakpoint
- Expected Result:
  - Menu switches to overlay mode without layout breakage
- Test Steps (continued):
  2. Expand viewport back to ≥ lg breakpoint
- Expected Result (continued):
  - Menu returns to persistent mode

---

### SCRUM-7: Menu behaves as overlay on small screens
**Test Case Title:** Overlay Menu Behavior on Small Screens
- Preconditions:
  - Viewport width is less than the lg breakpoint
- Test Steps:
  1. Load the application
- Expected Result:
  - The menu is hidden by default
- Test Steps (continued):
  2. Open the menu
- Expected Result (continued):
  - The menu displays as an overlay
- Test Steps (continued):
  3. Close the menu
- Expected Result (continued):
  - Focus returns to the previously focused element

---

### SCRUM-6: Split-pane shows persistent menu on large screens
**Test Case Title:** Persistent Menu in Split-Pane on Large Screens
- Preconditions:
  - Viewport width is ≥ the lg breakpoint
- Test Steps:
  1. Load the application
- Expected Result:
  - The menu is visible as a persistent left pane
  - The main content renders in the "main-content" outlet without overlaying the menu