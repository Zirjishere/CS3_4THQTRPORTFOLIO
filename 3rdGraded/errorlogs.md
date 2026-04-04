# Nlogonia Debugging - Errors


1. **File:** `script.js`  
   **Line:** 1  
   **Part:** JS  
   **Error:** The function `plotPoint()` had no parameters even though the button passes 4 arguments.  
   **How I corrected it:** I changed it to `function plotPoint(x0, y0, x, y)` so it receives all required values.

2. **File:** `script.js`  
   **Line:** 2  
   **Part:** JS  
   **Error:** Missing semicolon in `console.log(x0, y0, x, y)`.  
   **How I corrected it:** I added `;` to complete the statement properly.

3. **File:** `script.js`  
   **Line:** 7  
   **Part:** JS  
   **Error:** Used `point.styleleft`, which is not a valid style property access.  
   **How I corrected it:** I changed it to `point.style.left = ...`.

4. **File:** `script.js`  
   **Line:** 8  
   **Part:** JS  
   **Error:** Used `point.stylebottom`, which is not a valid style property access.  
   **How I corrected it:** I changed it to `point.style.bottom = ...`.

5. **File:** `script.js`  
   **Line:** End of function block  
   **Part:** JS  
   **Error:** Function block closure/braces were incorrect in the buggy version, causing parsing issues.  
   **How I corrected it:** I fixed the closing braces so `plotPoint` closes correctly with no extra brace.

6. **File:** `style.css`  
   **Line:** 35  
   **Part:** CSS  
   **Error:** Hover selector was written as `nav a :hover` (with space), which targets descendants incorrectly.  
   **How I corrected it:** I changed it to `nav a:hover`.

7. **File:** `style.css`  
   **Line:** 28  
   **Part:** CSS  
   **Error:** `nav a` used `display: block`, making links stack vertically instead of one line.  
   **How I corrected it:** I changed it to `display: inline-block` so links appear in one row.

8. **File:** `style.css`  
   **Line:** 22-25  
   **Part:** CSS  
   **Error:** Navigation was not fixed on top even if requirement says it should stay at top while scrolling.  
   **How I corrected it:** I added `position: fixed; top: 0; left: 0; z-index: 1000;` to `nav`.

9. **File:** `style.css`  
   **Line:** 94  
   **Part:** CSS  
   **Error:** Sprite URL pointed to wrong path (`sprites.png`) not matching actual folder structure.  
   **How I corrected it:** I changed it to `url('images/sprites.png')`.

10. **File:** `script.js`  
    **Line:** After creating `point`  
    **Part:** JS  
    **Error:** Point element needed absolute positioning so `left` and `bottom` values work reliably inside the plane.  
    **How I corrected it:** I added `point.style.position = 'absolute';`.

---

## Additional requirement updates completed

- In `3rdGraded/index.html`, I updated:
  - Author meta to `Zirjan Hero F. Mendaro`
  - Title to `CS 3 - Zirjan Hero F. Mendaro`
  - Header text to `Zirjan Hero F. Mendaro / 9 Rubidium - Mar 2026`

- In `3rdGraded/errorlogs.html`, I updated:
  - Author meta to `Zirjan Hero F. Mendaro`
  - Title to `CS3 - Zirjan Hero F. Mendaro`
  - Header text to `Zirjan Hero F. Mendaro / 9 Rubidium - Mar 2026`

- In root `index.html`, I added:
  - `Third Graded - Nlogonia Debugging` linking to `3rdGraded/index.html`
