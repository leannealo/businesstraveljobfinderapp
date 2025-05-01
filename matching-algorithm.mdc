# Skill Matching Algorithm

## Algorithm Overview
The matching algorithm ranks company categories based on user-selected skills and their rankings.

## Matching Process
1. Input Processing
   - User selects 5-25 skills from available list
   - User ranks top 5 skills in order of proficiency
   - Remaining selected skills treated as secondary matches

2. Category Matching
   - Compare user's top 5 skills against category requirements
   - Calculate match quality based on skill alignment
   - Consider secondary skills for tiebreaking

3. Ranking Logic
   Priority order for matches:
   1. Perfect matches (all 5 top skills)
   2. 4/5 top skills
   3. 3/5 top skills
   4. 2/5 top skills
   5. 1/5 top skills
   6. Matches with only secondary skills

## Match Quality Calculation
```javascript
function calculateMatchQuality(userSkills, categorySkills) {
  const topSkillMatches = countTopSkillMatches(userSkills.topFive, categorySkills);
  const secondaryMatches = countSecondaryMatches(userSkills.secondary, categorySkills);
  
  return {
    score: (topSkillMatches * 20) + (secondaryMatches * 5),
    topMatches: topSkillMatches,
    secondaryMatches: secondaryMatches
  };
}
```

## Output Generation
1. Sort categories by match quality
2. Take top 25 matching categories
3. For each category:
   - Include match quality score
   - List matching skills
   - Show associated companies

## Edge Cases
- Handle incomplete skill selections
- Account for tied scores
- Process categories with no matches
- Validate input data integrity
