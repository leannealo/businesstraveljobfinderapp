# Business Travel Job Finder App

## Overview
A web application to guide job seekers in the business travel industry by matching their skills to relevant company categories and suggesting companies to explore based on a provided spreadsheet.

## Requirements
- **User Interface**:
  - Question 1: Allow users to select a minimum of 5 and up to 25 transferable skills from a list of 25 (pulled from spreadsheet Tab 2).
  - Question 2: Prompt users to select and rank their top 5 skills (from those chosen in Question 1) from best to 5th best.
  - Display Results: Show 25 best-matching company categories with corresponding companies, ranked by skill match quality (perfect match to least matching).
- **Data Processing**:
  - Use spreadsheet data:
    - Tab 1: Company names.
    - Tab 2: List of 25 transferable skills.
    - Tab 3: Company categories.
    - Tab 4: Skills and categories mapping.
  - Match user-selected skills to categories based on Tab 4.
  - Rank matches: Start with perfect matches (all 5 top skills), then partial matches (4/5, 3/5, 2/5, 1/5, 0/5 but matching other selected skills), down to least matches.
  - Associate matched categories with companies from Tab 1 and Tab 3.
- **Output**:
  - List 25 category matches with their corresponding companies, sorted by match quality.
- **Constraints**:
  - Simple, user-friendly interface.
  - No local file I/O for spreadsheet; assume data is pre-loaded or fetched.
  - Handle edge cases (e.g., incomplete user input, no matches).

## Tech Stack
- **Frontend**: React with JSX for dynamic UI, Tailwind CSS for styling.
- **Backend**: None (client-side only, data processed in-browser).
- **Data Handling**: JavaScript for processing spreadsheet data (assumed as JSON or JS object).
- **Libraries**:
  - React (via CDN: cdn.jsdelivr.net).
  - Babel for JSX (via CDN).
- **Deployment**: Single-page HTML file, runs in any modern browser.

## Milestones
1. **Setup and Design**:
   - Create project structure with single HTML file.
   - Set up React and Tailwind CSS via CDN.
   - Design UI layout for questions and results display.
2. **Data Integration**:
   - Convert spreadsheet data to JSON/JS object format.
   - Load data into app (hard-coded or fetched).
3. **Question Flow**:
   - Implement Question 1: Multi-select for skills (min 5, max 25).
   - Implement Question 2: Top 5 skill ranking from selected skills.
   - Add input validation (e.g., enforce minimum selections).
4. **Matching Logic**:
   - Develop algorithm to match user skills to categories (using Tab 4).
   - Rank matches based on top 5 skills and additional selected skills.
   - Associate categories with companies (using Tabs 1 and 3).
5. **Results Display**:
   - Render 25 best matches with categories and companies.
   - Style results for clarity (e.g., highlight perfect matches).
6. **Testing and Refinement**:
   - Test with sample user inputs and edge cases.
   - Ensure responsive design and accessibility.
   - Refine UI/UX based on feedback.
7. **Finalization**:
   - Optimize performance (e.g., memoize calculations).
   - Document code and prepare for deployment.

## Notes
- Spreadsheet data should be pre-processed into a usable format (e.g., JSON) before integration.
- Focus on simplicity and usability for job seekers.
- Future enhancements could include backend API or dynamic data loading, but not in scope for initial version.
