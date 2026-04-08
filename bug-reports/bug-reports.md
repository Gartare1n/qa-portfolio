Title: BUG-01 Favorite button not working after closing login popup

Environment:
Browser: Brave (latest)
OS: macOS

Steps:
1. Open catalogue page
2. Click "Add to favorites"
3. Close login popup
4. Click again

Actual Result:
Button does not respond

Expected Result:
Login popup appears again or product is added after login

Severity: Medium  
Priority: Medium

***

Title: BUG-02 Catalogue sidebar closes when browser window is resized horizontally  

Environment:
Browser: Brave (latest)
OS: macOS

Steps:
1. Open homepage
2. Click "Catalogue" button in the top-left corner
3. Gradually decrease browser window width

Actual Result:
Catalogue sidebar closes automatically

Expected Result:
Catalogue sidebar remains visible and adjusts to screen size (responsive behavior)

Severity: Low  
Priority: Low

***

Title: BUG-03 Search input shifts due to hidden duplicate element in header on non-home pages  

Environment:
Browser: Brave (latest)
OS: macOS

Steps:
1. Open homepage
2. Observe header layout (logo, search bar, profile, cart)
3. Navigate to any other page
4. Compare header layout

Actual Result:
Search input shifts slightly to the left
Search field width is reduced

Expected Result:
Header layout remains consistent across all pages
Search input position and size do not change

Additional Info:
An extra hidden element with class "hidden md:d-block" appears in the DOM
This element affects layout spacing despite being invisible

Severity: Low  
Priority: Medium

***

Title: BUG-04 Search input accepts extremely large text causing UI break and performance issues  

Environment:
Browser: Brave (latest)
OS: macOS

Steps:
1. Open support section
2. Paste a very large text (~100,000+ characters) into the search input
3. Observe input field and search button

Actual Result:
- Page becomes slow and unresponsive
- Search button disappears visually
- Search functionality remains active but button is not visible

Expected Result:
- Input should have a reasonable character limit
- UI should remain stable
- Search button should remain visible and accessible

Additional Info:
No input length validation is applied
Issue may lead to performance degradation on low-end devices

Severity: Medium  
Priority: Medium

***

Title: BUG-05 Sorting dropdown text becomes hidden when multiple filters are applied  

Environment:
Browser: Brave (latest)
OS: macOS

Steps:
1. Open any section of the catalog
2. Apply multiple filters
3. Observe sorting dropdown element

Actual Result:
- Sorting dropdown shrinks
- Text label (e.g. "Sort by rating") becomes hidden
- Only dropdown icon remains visible

Expected Result:
- Sorting dropdown remains fully visible
- Text label is readable regardless of applied filters

Severity: Low  
Priority: Low

***

Title: BUG-06 "Personal data processing" link redirects to inaccessible Google Drive file  

Environment:
Browser: Brave (latest), Safari (latest)
OS: macOS

Steps:
1. Open login/registration popup
2. Locate the consent text at the bottom
3. Click on "Personal data processing" link

Actual Result: User is redirected to a Google Drive page with an error: "This file cannot be opened because it violates Google Drive Terms of Service"

Expected Result: User is redirected to a valid and accessible page with personal data processing policy

Severity: Medium  
Priority: High
