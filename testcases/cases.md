---
SCRUM-10: Navigating via secondary menu item routes correctly
Test Case Title: Secondary Menu Item Navigation
Preconditions: User is logged in and secondary menu items are visible.
Test Steps:
1. Verify the presence of a secondary menu item "<title>".
2. Click on the "<title>" menu item.
3. Observe navigation action.
4. Check if "<title>" menu item has "selected" active class.
Expected Result: Router navigates to "<url>" and the item "<title>" is marked as selected.
---
SCRUM-9: Navigating via primary menu item routes correctly and sets active state
Test Case Title: Primary Menu Item Navigation and Active State
Preconditions: User is logged in; primary menu items with icons are visible.
Test Steps:
1. Verify presence of primary menu item "<title>" with icon "<icon>".
2. Click the "<title>" menu item.
3. Observe navigation action.
4. Check "selected" active class on "<title>".
5. Ensure other menu items do not have "selected" class.
6. On mobile, confirm the menu closes and focus moves to main page heading.
Expected Result: Router navigates to "<url>", only the selected menu item is active, and mobile behavior is correct.
---
SCRUM-8: Switching between breakpoints recalculates the layout
Test Case Title: Responsive Layout Breakpoint Switching
Preconditions: App is open on a large screen (≥ lg breakpoint).
Test Steps:
1. Confirm app layout at large screen.
2. Shrink viewport below lg breakpoint.
3. Check if menu switches to overlay mode without breakage.
4. Expand viewport back to ≥ lg.
5. Verify menu returns to persistent mode.
Expected Result: Menu transitions correctly between overlay and persistent modes with no layout issues.
---
SCRUM-7: Menu behaves as overlay on small screens
Test Case Title: Overlay Menu Behavior on Small Screens
Preconditions: Viewport width is less than lg breakpoint; app is loaded.
Test Steps:
1. Load app with small viewport.
2. Check that menu is hidden by default.
3. Open the menu and verify it displays as overlay.
4. Close the menu and ensure focus returns to previously focused element.
Expected Result: Menu is hidden initially, appears as overlay when opened, and focus behavior is correct when closed.
---
SCRUM-6: Split-pane shows persistent menu on large screens
Test Case Title: Persistent Menu on Large Screens
Preconditions: Viewport width is ≥ lg breakpoint; app is loaded.
Test Steps:
1. Load app at large viewport width.
2. Confirm menu is visible as persistent left pane.
3. Check that main content renders in "main-content" outlet without overlaying menu.
Expected Result: Menu persists on the left and main content does not overlap with it.