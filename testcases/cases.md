SCRUM-10: Navigating via secondary menu item routes correctly
Test Case Title: Navigate via secondary menu item
Preconditions: User is logged in and secondary menu is visible.
Test Steps:
1. Verify presence of secondary menu item <title>.
2. Click the <title> menu item.
Expected Result:
- The router navigates to <url>.
- The item <title> has the "selected" active class.

SCRUM-9: Navigating via primary menu item routes correctly and sets active state
Test Case Title: Navigate via primary menu item and verify active state
Preconditions: User is logged in and primary menu is visible.
Test Steps:
1. Verify presence of primary menu item <title> with icon <icon>.
2. Click the <title> menu item.
Expected Result:
- The router navigates to <url>.
- The menu item <title> has the "selected" active class.
- All other menu items do not have the "selected" class.
- On mobile, the menu closes after navigation and focus moves to the main page heading.

SCRUM-8: Switching between breakpoints recalculates the layout
Test Case Title: Switch between breakpoints and verify layout recalculation
Preconditions: App is open on a large screen (viewport ≥ lg).
Test Steps:
1. Shrink viewport below lg breakpoint.
2. Expand viewport back to ≥ lg breakpoint.
Expected Result:
- Menu switches to overlay mode without layout breakage when below lg.
- Menu returns to persistent mode when back to ≥ lg.

SCRUM-7: Menu behaves as overlay on small screens
Test Case Title: Menu overlay behavior on small screens
Preconditions: Viewport width is less than lg breakpoint.
Test Steps:
1. Load the app.
2. Open the menu.
3. Close the menu.
Expected Result:
- Menu is hidden by default.
- Opening the menu displays it as an overlay.
- Closing themenu returns focus to the previously focused element.

SCRUM-6: Split-pane shows persistent menu on large screens
Test Case Title: Persistent split-pane menu on large screens
Preconditions: Viewport width is ₩ lg breakpoint.
Test Steps:
1. Load the app.
Expected Result:
- Menu is visible as a persistent left pane.
- Main content renders in the "main-content" outlet without overlaying the menu.