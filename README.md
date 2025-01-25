# Resolution Tracker DevOps Project

## Participants
- Amour Elias
- Benchabane Nahel
- Byl Ilias
- Meira Rolo Lucas

## 1. Introduction

### Context
People often make New Year's resolutions but struggle to maintain them beyond the first month. This project aims to solve this common challenge by creating an automated reminder and tracking system that provides consistent motivation throughout the year. When someone receives daily motivation and tracking, they are more likely to achieve their goals.

### Objectives
- Create an automated reminder system for monthly resolutions
- Provide timely notifications based on the date
- Track progress with weekly check-ins
- Offer encouragement and suggestions for each month's theme

## 2. Project Structure

### Architecture
```
project/
├── Jenkinsfile          # CI/CD pipeline configuration
└── README.md            # Project documentation
```

### Pipeline Stages
1. **Date Validation**
   - Validates input date
   - Extracts month and day information

2. **Monthly Resolution Stages**
   - January: Digital Diary
   - February: Home Improvement
   - March: Self-Care
   - April: Kindness
   - May: New Experiences
   - June: Family Time
   [Additional months to be implemented]

3. **Notification Summary**
   - Provides daily resolution summary
   - Tracks monthly progress

## 3. Monthly Resolutions

### January: Digital Diary
- **First Week Goal**: Journal setup
- **Daily Task**: Write daily reflections
- **Weekly Check**: Sunday reflection and goal tracking

### February: Home Redecoration
- **First Half**: Room selection and planning
- **Second Half**: Implementation of changes
- **Notifications**: Different messages before/after day 15

### March: Self-Care Journey
- **Daily Reminder**: Morning wellness routine
- **Weekly Check**: Routine adjustment and progress review
- **Focus**: Health habit formation

### April: Kindness Challenge
- **Daily Task**: Perform acts of kindness
- **Weekly Suggestions**: List of kind gestures
- **Tracking**: Weekly accomplishment review

### May: New Experiences
- **Early Month**: Adventure planning
- **Weekly Ideas**: New activity suggestions
- **Focus**: Stepping out of comfort zone

### June: Family Connections
- **Daily Focus**: Family time planning
- **Weekly Activities**: Family event suggestions
- **Goal**: Strengthening family bonds

[Additional months to be detailed...]

## 4. Implementation Details

### Jenkins Pipeline Features
- **Date Parameter**: Takes YYYY-MM-DD format
- **Conditional Execution**: Only runs relevant monthly stage
- **Progress Tracking**: Different messages based on day of month
- **Weekly Checks**: Special messages every 7 days

### Notification Types
1. **Daily Reminders**
   - Morning motivation
   - Task reminders
   - Progress checks

2. **Weekly Check-ins**
   - Progress summary
   - New suggestions
   - Achievement celebration

3. **Monthly Progress**
   - Mid-month motivation
   - End-of-month completion push

## 5. Usage Instructions

### Running the Pipeline
1. Open Jenkins dashboard
2. Select the Resolution Tracker pipeline
3. Click "Build with Parameters"
4. Enter current date (YYYY-MM-DD)
5. View console output for notifications

### Example Input
```
CURRENT_DATE: 2025-01-25
```

### Expected Output
- Monthly theme notification
- Daily task reminder
- Weekly check-in (if applicable)
- Progress status based on date

## 6. Future Improvements

### Planned Enhancements
- Implementation of remaining months (July-December)
- Additional weekly suggestions
- More detailed progress tracking
- Integration with notification systems

### Potential Features
- Mobile app integration
- Smart device connectivity
- Social sharing capabilities
- Achievement badges

## 7. Contributing
To contribute to this project:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request
4. Ensure pipeline tests pass

## 8. Contact
For questions or suggestions, contact team members:
- [Team member contact information]
