# React Component Architecture

## Component Structure
```
src/components/
├── SkillSelection/
│   ├── SkillList.jsx         # Multi-select skill interface (5-25 skills)
│   ├── SkillRanking.jsx      # Top 5 skill ranking interface
│   └── SelectedSkills.jsx    # Display and manage selected skills
├── Results/
│   ├── ResultsList.jsx       # Display 25 best matches
│   ├── CategoryCard.jsx      # Individual category display
│   └── CompanyList.jsx       # Companies within category
└── Common/
    ├── Button.jsx           # Reusable button component
    ├── Card.jsx            # Base card component
    └── ErrorBoundary.jsx   # Error handling wrapper
```

## Component Responsibilities

### SkillSelection Components
- `SkillList`: Handles selection of 5-25 skills from available options
- `SkillRanking`: Manages ranking of top 5 selected skills
- `SelectedSkills`: Shows current selection and validates requirements

### Results Components
- `ResultsList`: Displays and sorts matched categories
- `CategoryCard`: Shows category details and match quality
- `CompanyList`: Lists companies within each category

### Common Components
- Reusable UI components
- Consistent styling with Tailwind CSS
- Error boundary implementation

## Component Communication
- Props for parent-child communication
- Callback functions for user interactions
- No global state management (not required for this scope)

## Error Handling
- Input validation in skill selection
- Error boundaries for component failures
- User feedback for invalid selections
