# Status: Complete

All business requirements were fetched and the following test cases were generated for each, covering all relevant scenarios in the format of test case title, preconditions, test steps, and expected result:

---

## SCRUM-10: Navigating via secondary menu item routes correctly
- Test Case: Secondary Menu Navigation and Active State
- Preconditions: User is logged in and secondary menu is visible
- Steps:
  1. Verify a secondary menu item "<title>" is present
  2. Click the "<title>" menu item
- Expected: Router navigates to "<url>"; "<title>" menu item has the "selected" active class

---

## SCRUM-9: Navigating via primary menu item routes correctly and sets active state
- Test Case: Primary Menu Navigation and Active State (Desktop)
- Preconditions: User is logged in, primary menu visible, not mobile
- Steps:
  1. Verify a primary menu item "<title>" with icon "<icon>" is present
  2. Click the "<title>" menu item
- Expected: Router navigates to "<url>"; "<title>" has "selected" active class; other menu items do not; on mobile, menu closes after navigation and focus moves to main heading
- Test Case: Primary Menu Navigation Closes on Mobile and Focuses Heading
- Preconditions: User is logged in, primary menu visible, device is mobile
- Steps: Click the "<title>" menu item
- Expected: Router navigates to "<url>"; Menu closes after navigation; Focus moves to main page heading

---

## SCRUM-8: Switching between breakpoints recalculates the layout
- Test Case: Layout Recalculation on Breakpoint Shrink
- Preconditions: App is open on large screen (≥ lg)
- Steps: Shrink viewport below lg breakpoint
- Expected: Menu switches to overlay mode without layout breakage
- Test Case: Layout Returns to Persistent Mode on Breakpoint Expand
- Preconditions: Viewport previously shrunk below lg breakpoint, app running
- Steps: Expand viewport back to ≥ lg breakpoint
- Expected: Menu returns to persistent mode

---

## SCRUM-7: Menu behaves as overlay on small screens
- Test Case: Menu Hidden by Default on Small Screens
- Preconditions: Viewport width < lg breakpoint, app loaded
- Steps: Observe menu state after app load
- Expected: Menu hidden by default
- Test Case: Opening and Closing Overlay Menu Restores Focus on Small Screens
- Preconditions: Viewport width < lg breakpoint, app loaded, menu hidden by default
- Steps:
  1. Open menu (e.g., hamburger button)
  2. Close menu (e.g., close button or clicking outside)
- Expected: Opening displays overlay; closing returns focus to previously focused element

---

## SCRUM-6: Split-pane shows persistent menu on large screens
- Test Case: Persistent Menu Visibility on Large Screens
- Preconditions: Viewport width ≥ lg breakpoint, app loaded
- Steps: Observe left pane after app load
- Expected: Menu visible as persistent left pane
- Test Case: Main Content Renders Without Overlaying Menu on Large Screens
- Preconditions: Menu is persistent left pane, app loaded on large screen (≥ lg)
- Steps: Observe layout of main content area and menu pane after app load or navigation changes.
- Expected: Main content renders in the "main-content" outlet without overlaying the menu.
---