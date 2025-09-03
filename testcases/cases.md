SCRUM-10: Navigating via secondary menu item routes correctly
Test Case 1: Secondary menu item navigation
Preconditions:
- User is logged in and on a page displaying secondary menu items.
Test Steps:
1. Identify a visible secondary menu item labeled "<title>".
2. Click on the "<title>" menu item.
Expected Result:
- The router navigates to the URL "<url>" corresponding to the selected menu item.
- The "<title>" menu item displays the "selected" active class.

---
SCRUM-9: Navigating via primary menu item routes correctly and sets active state
Test Case 1: Primary menu item navigation and active state
Preconditions:
- User is logged in and on a page with primary menu items and icons.
Test Steps:
1. Locate a primary menu item labeled "<title>" with icon "<icon>".
2. Click on the "<title>" menu item.
Expected Result:
- The router navigates to the URL "<url>" for the selected menu item.
- The "<title>" menu item displays the "selected" active class.
- All other menu items do not display the "selected" class.
- On mobile, after navigation, the menu closes and focus moves to the main page heading.

---
SCRUM-8: Switching between breakpoints recalculates the layout
Test Case 1: Layout adapts when shrinking below large breakpoint
Preconditions:
- App is open on a large screen (viewport width ≥ lg breakpoint).
Test Steps:
1. Shrink viewport width below the lg breakpoint.
Expected Result:
- The menu switches to overlay mode without breaking the layout.
Test Case 2: Layout adapts when expanding above large breakpoint
Preconditions:
- Menu is in overlay mode due to small viewport.
Test Steps:
1. Expand viewport width back to ≥ lg breakpoint.
Expected Result:
- The menu returns to persistent mode.

---
SCRUM-7: Menu behaves as overlay on small screens
Test Case 1: Menu overlay behavior on small screens
Preconditions:
- Viewport width is less than the lg breakpoint.
Test Steps:
1. Load the application.
Expected Result:
- Menu is hidden by default.
Test Case 2: Opening and closing overlay menu
Preconditions:
- Menu is hidden by default on a small screen.
Test Steps:
1. Open the menu.
Expected Result:
- Menu displays as an overlay.
2. Close the menu.
Expected Result:
- Focus returns to the previously focused element.

---
SCRUM-6: Split-pane shows persistent menu on large screens
Test Case 1: Persistent split-pane menu display on large screens
Preconditions:
- Viewport width is ≥ lg breakpoint.
Test Steps:
1. Load the application.
Expected Result:
- Menu is visible as a persistent left pane.
- Main content renders in the "main-content" outlet without overlaying the menu.