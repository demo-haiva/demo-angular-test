### SCRUM-10: Navigating via secondary menu item routes correctly

**Test Case 1:**
- **Title:** Navigation through secondary menu item displays correct page
- **Preconditions:** User is on the application main page with secondary menu items visible
- **Test Steps:**
  1. Verify a secondary menu item "<title>" is visible
  2. Click on the "<title>" menu item
- **Expected Result:**
  - The router navigates to "<url>"
  - The item "<title>" has the "selected" active class

---

### SCRUM-9: Navigating via primary menu item routes correctly and sets active state

**Test Case 1:**
- **Title:** Primary menu navigation and active state
- **Preconditions:** User is on the application with primary menu items visible
- **Test Steps:**
  1. Verify a primary menu item "<title>" with icon "<icon>" is visible
  2. Click on the "<title>" menu item
- **Expected Result:**
  - The router navigates to "<url>"
  - The menu item "<title>" has the "selected" active class
  - All other menu items do not have the "selected" class
  - On mobile, the menu closes after navigation and focus moves to the main page heading

---

### SCRUM-8: Switching between breakpoints recalculates the layout

**Test Case 1:**
- **Title:** Responsive layout recalculation on breakpoint change
- **Preconditions:** App is open on a large screen
- **Test Steps:**
  1. Shrink viewport below the lg breakpoint
- **Expected Result:**
  - Menu switches to overlay mode without layout breakage
- **Test Steps (continued):**
  2. Expand viewport back to ≥ lg
- **Expected Result (continued):**
  - Menu returns to persistent mode

---

### SCRUM-7: Menu behaves as overlay on small screens

**Test Case 1:**
- **Title:** Overlay menu behavior on small screens
- **Preconditions:** Viewport width is less than lg breakpoint
- **Test Steps:**
  1. Load the app
- **Expected Result:**
  - Menu is hidden by default
- **Test Steps (continued):**
  2. Open the menu
- **Expected Result (continued):**
  - Menu displays as an overlay
- **Test Steps (continued):**
  3. Close the menu
- **Expected Result (continued):**
  - Focus returns to previously focused element

---

### SCRUM-6: Split-pane shows persistent menu on large screens

**Test Case 1:**
- **Title:** Persistent split-pane menu on large screens
- **Preconditions:** Viewport width is greater than or equal to lg breakpoint
- **Test Steps:**
  1. Load the app
- **Expected Result:**
  - Menu is visible as a persistent left pane
  - Main content renders in the "main-content" outlet without overlaying the menu,