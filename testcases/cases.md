SCRUM-10: Navigating via secondary menu item routes correctly
Test Case Title: Verify navigation via secondary menu item routes
Preconditions:
- User is logged in
- Secondary menu items are visible
Test Steps:
1. Identify a secondary menu item <title>
2. Click on the <title> menu item
Expected Result:
- The router navigates to <url>
- The item <title> has the "selected" active class

SCRUM-9: Navigating via primary menu item routes correctly and sets active state
Test Case Title: Verify navigation and active state of primary menu items
Preconditions:
- User is logged in
- Primary menu items with icons are visible
Test Steps:
1. Identify a primary menu item <title> with icon <icon>
2. Click on the <title> menu item
Expected Result:
- The router navigates to <url>
- The menu item <title> has the "selected" active class
- All other menu items do not have the "selected" class
- On mobile, the menu closes after navigation and focus moves to the main page heading

SCRUM-8: Switching between breakpoints recalculates the layout
Test Case Title: Verify layout recalculation on breakpoint changes
Preconditions:
- App is open on a large screen
Test Steps:
1. Shrink viewport below the lg breakpoint
2. Expand viewport back to ≥ lg breakpoint
Expected Result:
- Menu switches to overlay mode without layout breakage when shrunk below lg breakpoint
- Menu returns to persistent mode when expanded back to ≥ lg breakpoint

SCRUM-7: Menu behaves as overlay on small screens
Test Case Title: Verify overlay menu behavior on small screens
Preconditions:
- Viewport width is less than the lg breakpoint
Test Steps:
1. Load the app
2. Open the menu
3. Close the menu
Expected Result:
- Menu is hidden by default when app loads
- Opening the menu displays it as an overlay
- Closing the menu returns focus to the previously focused element

SCRUM-6: Split-pane shows persistent menu on large screens
Test Case Title: Verify persistent menu in split-pane layout on large screens
Preconditions:
- Viewport width is ≥ the lg breakpoint
Test Steps:
1. Load the app with large screen viewport
Expected Result:
- Menu is visible as a persistent left pane
- Main content renders in the "main-content" outlet without overlaying the menu,