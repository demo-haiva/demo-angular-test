SCRUM-10: Navigating via secondary menu item routes correctly
Test Case Title: Verify navigation and active state for secondary menu items
Preconditions: User is logged in and can view the secondary menu.
Test Steps:
1. Ensure a secondary menu item '<title>' is visible.
2. Click on the '<title>' menu item.
Expected Result:
- The router navigates to '<url>'.
- The item '<title>' has the 'selected' active class.

SCRUM-9: Navigating via primary menu item routes correctly and sets active state
Test Case Title: Verify navigation and active state for primary menu items
Preconditions: User is logged in; primary menu is visible with icons.
Test Steps:
1. Ensure a primary menu item '<title>' with icon '<icon>' is visible.
2. Click on the '<title>' menu item.
Expected Result:
- The router navigates to '<url>'.
- The menu item '<title>' has the 'selected' active class.
- All other menu items do not have the 'selected' class.
- On mobile, the menu closes after navigation and focus moves to the main page heading.

SCRUM-8: Switching between breakpoints recalculates the layout
Test Case Title: Layout recalculation on breakpoint change
Preconditions: App is open on a large screen.
Test Steps:
1. Shrink viewport below lg breakpoint.
2. Expand viewport back to ≥ lg breakpoint.
Expected Result:
- Menu switches to overlay mode without layout breakage.
- Menu returns to persistent mode when viewport expands.

SCRUM-7: Menu behaves as overlay on small screens
Test Case Title: Overlay behavior of menu on small screens
Preconditions: Viewport width is less than lg breakpoint.
Test Steps:
1. Load the app.
2. Open the menu.
3. Close themenu.
Expected Result:
- Menu is hidden by default.
- Opening the menu displays it as an overlay.
- Closing themenu returns focus to the previously focused element.

SCRUM-6: Split-pane shows persistent menu on large screens
Test Case Title: Persistent left pane on large screens
Preconditions: Viewport width is ≥ lg breakpoint; app loads successfully.
Test Steps:
1. Load the app with a large viewport.
Expected Result:
- Menu is visible as a persistent left pane.
- Main content renders in 'main-content'outlet without overlaying the menu.