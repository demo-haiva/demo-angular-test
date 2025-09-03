**SCRUM-10: Navigating via secondary menu item routes correctly**
Test Case Title: Navigating via secondary menu item routes
Preconditions: User is logged in and can see the application menu.
Test Steps:
1. Ensure the secondary menu item "<title>" is visible.
2. Click the "<title>" menu item.
Expected Result:
- The router navigates to "<url>".
- The item "<title>" has the "selected" active class.

---

**SCRUM-9: Navigating via primary menu item routes correctly and sets active state**
Test Case Title: Navigating via primary menu item routes and active state
Preconditions: User is logged in and the application is open on desktop or mobile.
Test Steps:
1. Verify a primary menu item "<title>" with icon "<icon>" is visible.
2. Click the "<title>" menu item.
Expected Result:
- The router navigates to "<url>".
- The menu item "<title>" has the "selected" active class.
- All other menu items do not have the "selected" class.
- On mobile, the menu closes after navigation and focus moves to the main page heading.

---

**SCRUM-8: Switching between breakpoints recalculates the layout**
Test Case Title: Layout recalculation on breakpoint switch
Preconditions: App is open on a large screen (≥ lg breakpoint).
Test Steps:
1. Shrink the viewport below the lg breakpoint.
2. Observe the menu behavior.
3. Expand the viewport back to ≥ lg.
Expected Result:
- Menu switches to overlay mode without layout breakage when below lg breakpoint.
- Menu returns to persistent mode when expanded back to ≥ lg.

---

**SCRUM-7: Menu behaves as overlay on small screens**
Test Case Title: Overlay menu behavior on small screens
Preconditions: Viewport width is less than the lg breakpoint.
Test Steps:
1. Load the app.
2. Open the menu.
3. Close the menu.
Expected Result:
- Menu is hidden by default on load.
- Opening displays it as an overlay.
- Closing returns focus to previously focused element.

---

**SCRUM-6: Split-pane shows persistent menu on large screens**
Test Case Title: Persistent split-pane menu on large screens
Preconditions: Viewport width is greater than or equal to the lg breakpoint.
Test Steps:
1. Load the app.
Expected Result:
- Menu is visible as a persistent left pane.
- Main content renders in the "main-content" outlet without overlaying the menu.