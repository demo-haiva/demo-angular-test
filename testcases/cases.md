### SCRUM-10: Navigating via secondary menu item routes correctly
**Test Case Title:** Navigation via Secondary Menu Item
- **Preconditions:** User is logged in and secondary menu is visible.
- **Test Steps:**
  1. Ensure a secondary menu item "<title>" is present.
  2. Click the "<title>" menu item.
- **Expected Result:**
  - The router navigates to "<url>".
  - The item "<title>" has the "selected" active class.

---
### SCRUM-9: Navigating via primary menu item routes correctly and sets active state
**Test Case Title:** Navigation via Primary Menu Item and Active State
- **Preconditions:** User is logged in and primary menu is visible with items and icons.
- **Test Steps:**
  1. Ensure a primary menu item "<title>" with icon "<icon>" is present.
  2. Click the "<title>" menu item.
- **Expected Result:**
  - The router navigates to "<url>".
  - The menu item "<title>" has the "selected" active class.
  - All other menu items do not have the "selected" class.
  - On mobile, the menu closes after navigation and focus moves to the main page heading.

---
### SCRUM-8: Switching between breakpoints recalculates the layout
**Test Case Title:** Layout Recalculation on Breakpoint Change
- **Preconditions:** Application is open on a large screen.
- **Test Steps:**
  1. Open the app on a large screen (≥ lg breakpoint).
  2. Shrink the viewport below the lg breakpoint.
- **Expected Result:**
  - The menu switches to overlay mode without layout breakage.
  3. Expand the viewport back to ≥ lg.
- **Expected Result:**
  - The menu returns to persistent mode.

---
### SCRUM-7: Menu behaves as overlay on small screens
**Test Case Title:** Overlay Menu on Small Screens
- **Preconditions:** Device viewport width is less than the lg breakpoint.
- **Test Steps:**
  1. Load the application.
- **Expected Result:**
  - The menu is hidden by default.
  2. Open the menu.
- **Expected Result:**
  - The menu displays as an overlay.
  3. Close the menu.
- **Expected Result:**
  - Focus returns to the previously focused element.

---
### SCRUM-6: Split-pane shows persistent menu on large screens
**Test Case Title:** Persistent Menu on Large Screens (Split-pane)
- **Preconditions:** Device viewport width is ≥ the lg breakpoint.
- **Test Steps:**
  1. Load the application.
- **Expected Result:**
  - The menu is visible as a persistent left pane.
  - The main content renders in the "main-content" outlet without overlaying the menu.