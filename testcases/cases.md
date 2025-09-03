1. SCRUM-10: Navigating via secondary menu item routes correctly
Test Case Title: Navigation using secondary menu item routes
Preconditions: User is logged in and can view the application with a visible secondary menu.
Test Steps: (1) Locate a secondary menu item labeled "<title>". (2) Click on the "<title>" menu item.
Expected Result: The router navigates to "<url>". The item "<title>" has the "selected" active class applied.

2. SCRUM-9: Navigating via primary menu item routes correctly and sets active state
Test Case Title: Navigation and active state for primary menu items
Preconditions: User is logged in and the primary menu is visible.
Test Steps: (1) Locate a primary menu item labeled "<title>" with icon "<icon>". (2) Click on the "<title>" menu item.
Expected Result: The router navigates to "<url>". The menu item "<title>" has the "selected" active class applied. All other menu items do not have the "selected" class. On mobile, after navigation, the menu closes and focus moves to the main page heading.

3. SCRUM-8: Switching between breakpoints recalculates the layout
Test Case Title: Responsive layout recalculation between breakpoints
Preconditions: Application is open on a large screen (≥ lg breakpoint).
Test Steps: (1) Shrink the viewport below the lg breakpoint. (2) Observe the menu behavior. (3) Expand the viewport back to ≥ lg breakpoint.
Expected Result: The menu switches to overlay mode without layout breakage when shrinking below lg. The menu returns to persistent mode when expanding back to ≥ lg.

4. SCRUM-7: Menu behaves as overlay on small screens
Test Case Title: Overlay menu behavior on small screens
Preconditions: Viewport width is less than the lg breakpoint.
Test Steps: (1) Load the application. (2) Open the menu. (3) Close the menu.
Expected Result: The menu is hidden by default on load. Opening the menu displays it as an overlay. Closing the menu returns focus to the previously focused element.

5. SCRUM-6: Split-pane shows persistent menu on large screens
Test Case Title: Persistent split-pane menu on large screens
Preconditions: Viewport width is at least the lg breakpoint.
Test Steps: (1) Load the application. (2) Observe the left pane and main content area.
Expected Result: The menu is visible as a persistent left pane. The main content renders in the "main-content" outlet without overlaying the menu.