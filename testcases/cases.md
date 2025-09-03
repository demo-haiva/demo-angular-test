---
SCRUM-10: Navigating via secondary menu item routes correctly
Test Case Title: Navigation via secondary menu item
Preconditions: User is on a page with a visible secondary menu
Test Steps:
1. Locate the secondary menu item "<title>"
2. Click the "<title>" menu item
Expected Result:
- The router navigates to "<url>"
- The item "<title>" has the "selected" active class
---
SCRUM-9: Navigating via primary menu item routes correctly and sets active state
Test Case Title: Navigation via primary menu item and active state verification
Preconditions: User is on a page with a visible primary menu
Test Steps:
1. Verify primary menu item "<title>" with icon "<icon>" is visible
2. Click the "<title>" menu item
Expected Result:
- The router navigates to "<url>"
- The menu item "<title>" has the "selected" active class
- All other menu items do not have the "selected" class
- On mobile, the menu closes after navigation and focus moves to the main page heading
---
SCRUM-8: Switching between breakpoints recalculates the layout
Test Case Title: Layout recalculation on breakpoint change
Preconditions: App is open on a large screen
Test Steps:
1. Shrink viewport below the lg breakpoint
Expected Result:
- Menu switches to overlay mode without layout breakage
2. Expand viewport back to ≥ lg
Expected Result:
- Menu returns to persistent mode
---
SCRUM-7: Menu behaves as overlay on small screens
Test Case Title: Overlay menu behavior on small screens
Preconditions: Viewport width is less than lg breakpoint
Test Steps:
1. Load the app
Expected Result:
- Menu is hidden by default
2. Open the menu
Expected Result:
- Menu displays as an overlay
3. Close the menu
Expected Result:
- Focus returns to previously focused element
---
SCRUM-6: Split-pane shows persistent menu on large screens
Test Case Title: Persistent split-pane menu on large screens
Preconditions: Viewport width is ≥ lg breakpoint
Test Steps:
1. Load the app
Expected Result:
- Menu is visible as a persistent left pane
- Main content renders in the "main-content" outlet without overlaying the menu
---