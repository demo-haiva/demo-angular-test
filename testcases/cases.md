**1. SCRUM-10: Navigating via secondary menu item routes correctly**
Test Case Title: Navigate via secondary menu item and validate route
Preconditions: User is logged in and on the main page with secondary menu items visible.
Test Steps:
1. Verify the presence of a secondary menu item "<title>".
2. Click on the "<title>" menu item.
Expected Result:
- The router navigates to "<url>".
- The item "<title>" has the "selected" active class.

---

**2. SCRUM-9: Navigating via primary menu item routes correctly and sets active state**
Test Case Title: Navigate via primary menu item and verify active state
Preconditions: User is logged in and on the main page with primary menu items visible.
Test Steps:
1. Confirm presence of primary menu item "<title>" with icon "<icon>".
2. Click on the "<title>" menu item.
Expected Result:
- The router navigates to "<url>".
- The menu item "<title>" has the "selected" active class.
- All other menu items do not have the "selected" class.
- On mobile, the menu closes after navigation and focus moves to the main page heading.

---

**3. SCRUM-8: Switching between breakpoints recalculates the layout**
Test Case Title: Layout recalculates correctly on breakpoint changes
Preconditions: App is open on a large screen (viewport ≥ lg breakpoint).
Test Steps:
1. Shrink viewport below the lg breakpoint.
2. Expand viewport back to ≥ lg.
Expected Result:
- Menu switches to overlay mode without layout breakage when shrinking.
- Menu returns to persistent mode when expanding back.

---

**4. SCRUM-7: Menu behaves as overlay on small screens**
Test Case Title: Overlay menu behavior on small screens
Preconditions: Viewport width is less than the lg breakpoint.
Test Steps:
1. Load the app.
2. Open the menu.
3. Close the menu.
Expected Result:
- Menu is hidden by default.
- Opening themenu displays it as an overlay.
- Closing themenu returns focus to the previously focused element.

---

**5. SCRUM-6: Split-pane shows persistent menu on large screens**
Test Case Title: Persistent menu display on large screens
Preconditions: Viewport width is greater than or equal to the lg breakpoint.
Test Steps:
1.Load the app.
ExpectedResult:
- Menu is visible as a persistent left pane.
- Main content renders in the "main-content" outlet without overlaying the menu.