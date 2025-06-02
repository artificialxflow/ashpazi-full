# Bolt Automation Instructions

This file contains explicit step-by-step instructions for Bolt. When Bolt reads this file, it must follow these instructions in order to automate the Figma-to-code workflow for this repository.

---

## Instructions for Bolt

1. **On Startup**
   - Read this `todo.md` file for instructions before taking any action.

2. **Repository Structure**
   - For each folder in the repository (excluding system and config folders):
     - Check if the folder contains:
       - A text file with the Figma design link(s)
       - A screenshot image of the page/component
       - All required icons and images (PNG/SVG/JPG)
     - If any required file is missing, prompt the user to provide it and pause processing for that folder until all assets are present.

3. **Page Generation**
   - For each folder with all required assets:
     1. Read the Figma link from the text file.
     2. Use the screenshot and all provided images/icons as reference.
     3. Generate an `index.html` file in the same folder that:
        - Implements the design as shown in the screenshot and Figma link.
        - Uses Bootstrap for layout and styling.
        - Uses provided CSS and images.
        - Adds JavaScript if needed for interactivity.
        - Ensures the implementation matches the Figma design as closely as possible.
     4. If any additional information or asset is needed, prompt the user and wait for input before continuing.

4. **Repeat**
   - Repeat the above steps for every folder representing a page or component.

5. **Completion**
   - When all folders have a completed `index.html` matching the Figma design, notify the user.

---

## Checklist for Bolt

- [ ] Read this file on startup
- [ ] Process each folder as described
- [ ] Prompt user for missing assets or information
- [ ] Generate `index.html` using Bootstrap and provided assets
- [ ] Ensure pixel-perfect match to Figma design
- [ ] Notify user when all pages/components are complete

---

**Bolt must follow these instructions exactly. Update this file if the workflow changes.** 