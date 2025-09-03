SCRUM-10: Navigating via secondary menu item routes correctly
Test Case Title: Navigate via secondary menu item and validate route & active state
Preconditions: User is logged in and can see the application menu
Test Steps:
1. Verify that a secondary menu item <title> is visible
2. Click the <title> menu item
Expected Result:
- Router navigates to <url>
- The item <title> has the "selected" active class

SCRUM-9: Navigating via primary menu item routes correctly and sets active state
Test Case Title: Navigate via primary menu item, validate active state, and mobile behavior
Preconditions: User is logged in and on a device (desktop/mobile)
Test Steps:
1. Verify that a primary menu item <title> with icon <icon> is visible
2. Click the <title> menu item
Expected Result:
- Router navigates to <url>
- The menu item <title> has the "selected" active class
- All other menu items do not have the "selected" class
- On mobile, the menu closes after navigation and focus moves to the main page heading

SCRUM-8: Switching between breakpoints recalculates the layout
Test Case Title: Switch between breakpoints and validate layout recalculation
Preconditions: App is open on a large screen
Test Steps:
1. Shrink the viewport below the lg breakpoint
Expected Result:
- Menu switches to overlay mode without layout breakage
2. Expand the viewport back to ≥ lg
Expected Result:
- Menu returns to persistent mode

SCRUM-7: Menu behaves as overlay on small screens
Test Case Title: Validate menu overlay behavior on small screens
Preconditions: Device viewport width is less than lg breakpoint
Test Steps:
1. Load the app
Expected Result:
- Menu is hidden by default
2. Open the menu
Expected Result:
- Menu displays as an overlay
3. Close the menu
Expected Result:
- Focus returns to the previously focused element

SCRUM-6: Split-pane shows persistent menu on large screens
Test Case Title: Validate persistent menu in split-pane on large screens
Preconditions: Device viewport width is greater than or equal to lg breakpoint
Test Steps:
1. Load the app
Expected Result:
- Menu is visible as a persistent left pane
- Main content renders in the "main-content" outlet without overlaying the menu,