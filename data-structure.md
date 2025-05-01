# Data Structure and Integration

## Spreadsheet Data Organization
The application uses data from 4 key spreadsheet tabs that will be converted to JSON:

### Tab Structure
1. Companies Tab
   - Company names and basic information
   - Will be stored in `src/data/companies.json`

2. Skills Tab
   - List of 25 transferable skills
   - Will be stored in `src/data/skills.json`

3. Categories Tab
   - Company categories/industries
   - Will be stored in `src/data/categories.json`

4. Mapping Tab
   - Skills to categories mapping data
   - Will be stored in `src/data/skill-category-mapping.json`

## Data Integration
- Data will be pre-processed into JSON format
- No runtime file I/O operations
- Data loaded and cached on initial app load
- Optimized for quick skill matching operations

## Data Flow
1. Load pre-processed JSON data on app initialization
2. User selects and ranks skills
3. Match skills against category mapping
4. Filter and rank companies based on matches
5. Display top 25 matches with company information

## Data Security
- All data stored client-side
- No sensitive information in pre-processed data
- No external API calls required
