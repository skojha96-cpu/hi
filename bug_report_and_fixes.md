# Bug Report and Fixes for Exam Management System

## Bug Report

### 1. Print/Preview Discrepancies
**Issue:** The print and preview functionality do not match the on-screen display of the exam management system. Elements are misaligned, and some data does not appear in the printed version.
**Steps to Reproduce:**  
1. Navigate to the exam management system page.  
2. Click on the print/preview button.  
3. Compare the output with the on-screen display.  

**Expected Result:** Print and preview should match the displayed data without discrepancies.

**Fix:**  
- Review CSS styles affecting layout during print media.  
- Ensure all relevant elements are included in the print stylesheet.

### 2. Data Persistence Issues
**Issue:** Data entered in the forms does not persist after navigation away from the page or upon refresh.
**Steps to Reproduce:**  
1. Fill out an exam form.  
2. Click on a different page within the system.  
3. Return to the exam form page and observe that the previously filled data is lost.

**Expected Result:** Data should remain in the form after navigating away.

**Fix:**  
- Implement local storage to save form data temporarily.  
- Use JavaScript to populate the form with saved data upon return.

### 3. UI Bugs
**Issue:** Several UI elements do not function as intended or appear misaligned.
  - Buttons overlap with text on certain screen sizes.  
  - Dropdown menus are unresponsive in mobile view.

**Steps to Reproduce:**  
1. Access the exam management system on various devices (desktop, tablet, mobile).  
2. Observe button and dropdown menu behavior.

**Expected Result:** All UI elements should be functional and appropriately responsive.

**Fix:**  
- Use media queries to adjust styles for different screen sizes.  
- Ensure that JavaScript events are properly bound for dropdown functionality across devices.

## Conclusion
Addressing these issues will improve the functionality, user experience, and reliability of the exam management system. A series of testing activities should follow the implementation of these fixes to ensure all issues are resolved before deployment.
