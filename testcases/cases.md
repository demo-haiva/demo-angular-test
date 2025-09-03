# Test Cases for Selected Business Requirements

---

## SCRUM-10: Navigating via secondary menu item routes correctly
**Test Case Title:** Secondary Menu Item Navigation
**Preconditions:** User is logged in and secondary menu is visible.
**Test Steps:**
1. Identify a secondary menu item labeled "<title>".
2. Click on the "<title>" menu item.
**Expected Result:**
- The router navigates to "<url>".
- The item "<title>" has the "selected" active class.

---

## SCRUM-9: Navigating via primary menu item routes correctly and sets active state
**Test Case Title:** Primary Menu Item Navigation and Active State
**Preconditions:** User is logged in and primary menu is visible.
**Test Steps:**
1. Identify a primary menu item labeled "<title>" with icon "<icon>".
2. Click on the "<title>" menu item.
**Expected Result:**
- The router navigates to "<url>".
- The menu item "<title>" has the "selected" active class.
- All other menu items do not have the "selected" class.
- On mobile, after navigation, the menu closes and focus moves to the main page heading.

---

## SCRUM-8: Switching between breakpoints recalculates the layout
**Test Case Title:** Responsive Layout Switch on Breakpoint Change
**Preconditions:** Application is open on a large screen.
**Test Steps:**
1. Shrink viewport below the lg breakpoint.
2. Expand viewport back to ≥ lg.
**Expected Result:**
- Menu switches to overlay mode without layout breakage when shrunk below lg breakpoint.
- Menu returns to persistent mode when expanded back to ≥ lg.

---

## SCRUM-7: Menu behaves as overlay on small screens
**Test Case Title:** Overlay Menu on Small Screens
**Preconditions:** Device viewport width is less than the lg breakpoint.
**Test Steps:**
1. Load the application.
2. Open the menu.
3. Close the menu.
**Expected Result:**
- The menu is hidden by default.
- Opening the menu displays it as an overlay.
- Closing the menu returns focus to the previously focused element.

---

## SCRUM-6: Split-pane shows persistent menu on large screens
**Test Case Title:** Persistent Menu on Large Screens (Split-Pane)
**Preconditions:** Device viewport width is ≥ the lg breakpoint.
**Test Steps:**
1. Load the application.
**Expected Result:**
- The menu is visible as a persistent left pane.
- The main content renders in the "main-content" outlet without overlaying the menu.
