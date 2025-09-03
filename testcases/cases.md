### SCRUM-10: Navigating via secondary menu item routes correctly
Test Case 1: Navigation through Secondary Menu Item
Preconditions: User is logged in and can view the secondary menu.
Test Steps:
1. Identify a secondary menu item labeled "<title>".
2. Click the "<title>" menu item.
Expected Result:
- The application navigates to the corresponding "<url>".
- The "<title>" menu item is marked with the "selected" active class.

---

### SCRUM-9: Navigating via primary menu item routes correctly and sets active state
Test Case 1: Navigation through Primary Menu Item
Preconditions: User is logged in and can view the primary menu.
Test Steps:
1. Locate a primary menu item labeled "<title>" with icon "<icon>".
2. Click the "<title>" menu item.
Expected Result:
- The application navigates to the correct "<url>".
- The selected menu item has the "selected" active class.
- All other menu items do not have the "selected" class.
Test Case 2: Mobile Navigation Closes Menu and Sets Focus
Preconditions: User is on a mobile device.
Test Steps:
1. Tap a primary menu item.
Expected Result:
- The menu closes after navigation.
- Focus moves to the main page heading.

---

### SCRUM-8: Switching between breakpoints recalculates the layout
Test Case 1: Layout Adapts on Breakpoint Change
Preconditions: App is open on a large screen (≥ lg breakpoint).
Test Steps:
1. Shrink viewport below the lg breakpoint.
Expected Result:
- The menu switches to overlay mode without layout breakage.
Test Case 2: Layout Returns to Persistent Mode
Preconditions: App is in overlay mode (viewport < lg breakpoint).
Test Steps:
1. Expand viewport back to ≥ lg breakpoint.
Expected Result:
- The menu returns to persistent mode.

---

### SCRUM-7: Menu behaves as overlay on small screens
Test Case 1: Menu Hidden by Default on Small Screens
Preconditions: Viewport width is less than the lg breakpoint.
Test Steps:
1. Load the application.
Expected Result:
- The menu is hidden by default.
Test Case 2: Opening Menu Displays as Overlay
Preconditions: Application is loaded on a small screen.
Test Steps:
1. Open the menu.
Expected Result:
- The menu displays as an overlay.
Test Case 3: Closing Menu Returns Focus
Preconditions: Menu is open as an overlay.
Test Steps:
1. Close the menu.
Expected Result:
- Focus returns to the previously focused element.

---

### SCRUM-6: Split-pane shows persistent ment on large screens
Test Case 1: Persistent Menu on Large Screens
Preconditions: Viewport width is ≥ lg breakpoint.
Test Steps:
1. Load the application.
Expected Result:
- The menu is visible as a persistent left pane.
- The main content renders in the "main-content" outlet without overlaying the menu.