# Indpro Manager - InMa

## Project Overview

We are creating a management solution for running internal operations in Indpro. It is super important as we are losing a lot of money and time doing management manually. This should be a very slim solution to start with and ready to be scalable.

**This is a competitive assessment to find the best talent who can design this solution for us. Whoever gets the most of it done will be rewarded for exceptional work.**

⚠️ **Important**: This assessment should not affect your daily general work responsibilities.

## Getting Started

### How to Use This Template (Step-by-Step Instructions)

**Step 1: Create Your Own Repository from This Template**
1. Make sure you are logged into your GitHub account
2. At the top of this repository page, you will see a green button that says **"Use this template"**
3. Click on **"Use this template"** button
4. Click on **"Create a new repository"** from the dropdown menu
5. You will be taken to a new page to create your repository

**Step 2: Configure Your New Repository**
1. **Repository name**: Enter exactly this format: `inma-assessment-[your-full-name]-[current-date]`
   - Replace `[your-full-name]` with your actual name (use hyphens instead of spaces)
   - Replace `[current-date]` with today's date in YYYY-MM-DD format
   - ✅ **Good example**: `inma-assessment-john-smith-2024-06-24`
   - ❌ **Bad example**: `my-project` or `inma-test`

2. **Repository visibility**: 
   - VERY IMPORTANT: Select **"Private"** (not Public)
   - This ensures other candidates cannot see your work
   - If you accidentally make it public, go to Settings → General → Danger Zone → Change visibility

3. **Include all branches**: Leave this checked (it's usually checked by default)

4. Click the green **"Create repository"** button at the bottom

**Step 3: Set Up Your Local Development Environment**

*If you're new to Git and GitHub, follow these detailed steps:*

1. **Install Git on your computer** (if not already installed):
   - Windows: Download from [git-scm.com](https://git-scm.com/)
   - Mac: Install via Terminal: `xcode-select --install`
   - Linux: `sudo apt-get install git` (Ubuntu) or equivalent for your distro

2. **Clone your repository to your computer**:
   - On your new repository page on GitHub, click the green **"Code"** button
   - Copy the HTTPS URL (it will look like: `https://github.com/yourusername/inma-assessment-yourname-date.git`)
   - Open Terminal/Command Prompt on your computer
   - Navigate to where you want to store the project: `cd Desktop` (or wherever you prefer)
   - Run: `git clone [paste-the-url-you-copied]`
   - Example: `git clone https://github.com/johndoe/inma-assessment-john-smith-2024-06-24.git`

3. **Navigate into your project folder**:
   ```bash
   cd inma-assessment-[your-name]-[date]
   ```

**Step 4: Verify Everything is Set Up Correctly**
1. Open the project folder in your favorite code editor (VS Code, Sublime Text, etc.)
2. You should see this README.md file and the basic folder structure
3. Run `git status` in your terminal - it should show you're on the main branch with no changes

**Step 5: Start Working on the Assessment**
1. **Create a development branch** (recommended):
   ```bash
   git checkout -b development
   ```
2. Start building according to the requirements below
3. **Commit your changes regularly** (at least once per day):
   ```bash
   git add .
   git commit -m "Add user authentication feature"
   git push origin development
   ```

**Step 6: Final Submission**
1. **Create your final README**: Replace this template README with your own that includes:
   - How to install and run your project
   - Environment setup instructions
   - API documentation
   - Any special features you implemented

2. **Push all your final changes**:
   ```bash
   git add .
   git commit -m "Final submission - completed assessment"
   git push origin development
   ```

3. **Create a Pull Request**:
   - Go to your repository on GitHub
   - Click "Compare & pull request" button
   - Title it: "Assessment Submission - [Your Name]"
   - In the description, briefly explain what you built and any special instructions

4. **Share repository access**:
   - Go to your repository Settings → Manage access
   - Click "Invite a collaborator"
   - Add the email addresses provided by HR/Technical Lead
   - This allows us to review your private repository

### Troubleshooting Common Issues

**"I can't find the 'Use this template' button"**
- Make sure you're logged into GitHub
- The button is green and located at the top right of the repository page
- If you still can't see it, try refreshing the page

**"My repository is showing as public"**
- Go to your repository Settings
- Scroll down to "Danger Zone"
- Click "Change repository visibility"
- Select "Make private"

**"Git commands are not working"**
- Make sure Git is installed on your computer
- Check that you're in the correct folder using `pwd` (Mac/Linux) or `cd` (Windows)
- Verify the repository URL is correct

**"I made a mistake in my repository name"**
- Go to your repository Settings
- At the top, you can rename your repository
- Make sure to follow the naming convention exactly

**Need help with Git commands?**
- `git status` - See what files have changed
- `git add .` - Add all changes to staging
- `git commit -m "your message"` - Save changes with a message
- `git push` - Upload changes to GitHub
- `git pull` - Download latest changes from GitHub

### What You Need Before Starting
- A GitHub account (free)
- A code editor (VS Code recommended - it's free)
- Git installed on your computer
- Basic knowledge of command line/terminal
- Your preferred programming languages and frameworks installed

## Business Context

We are a software consulting company, and the two most important things we handle every day are **projects** and **employees**. This solution needs to streamline our project management and resource allocation processes.

## Technical Requirements

### Core Entities
You need to build a system with two main entities:
- **Projects** - Software projects that the company works on
- **Users** - Employees who work on these projects

### 1. Projects Module

#### A. Projects List View (Main Projects Page)
Create a page that shows all projects in a table format. This table must include:

**Required Table Columns** (use your judgment for additional ones):
- Project Name
- Start Date
- End Date
- Status (Active, Completed, On Hold, etc.)
- Assigned Team Members (count or names)
- Progress Percentage
- GitHub/Bitbucket Repository Links
- Last Updated Date

**Required Functionality:**
- **Search Bar**: Users can search projects by name
- **Filter Options**: Filter by status, date range, assigned users
- **Sorting**: Click column headers to sort ascending/descending
- **Pagination**: If you have many projects, show 10-20 per page
- **Action Buttons**: Edit, Delete, View Details for each project

#### B. Project Detail Page (Individual Project Dashboard)
When someone clicks on a project from the list, show a detailed dashboard page with these specific sections:

**Section 1: Top Statistics Cards (4 Cards Side by Side)**
Create 4 cards that display:
1. **Tickets Closed**: Total number of completed Jira tickets
2. **Tickets In Progress**: Tickets currently being worked on
3. **Tickets Not Started**: Tickets in backlog/to-do status
4. **Tickets Left**: Total remaining tickets (In Progress + Not Started)

Each card should show:
- Large number (the count)
- Small descriptive text
- Different background colors for each card

**Section 2: Analytics Charts**
- **Time Period Selector**: Dropdown to choose "Last 3 Months", "Last 6 Months", "Last Year", "All Time"
- **Chart**: Line graph or bar chart showing ticket completion over time
- **User Filter**: Dropdown to filter the chart by specific team member or "All Users"
- **Legend**: Show what each line/bar represents

**Section 3: Team Section**
Display in a table or cards:
- List of all users assigned to this project
- For each user show:
  - Name and profile picture (if available)
  - Allocation percentage (e.g., "50%" means they work half-time on this project)
  - Number of tickets they completed for this project
  - Their current active tickets for this project

#### C. Project Creation & Management

**Create New Project Page:**
Build a form with these required fields:
- **Project Name**: Text input (required)
- **Description**: Textarea for project description
- **Start Date**: Date picker
- **End Date**: Date picker  
- **GitHub Repository URL**: Text input for repository link
- **Bitbucket Repository URL**: Text input (alternative to GitHub)
- **Project Manager**: Dropdown to select a user
- **Initial Team Members**: Multi-select dropdown of users

**Admin-Only Features** (implement basic admin role):
- **Dynamic Fields**: Admin can add custom fields to projects (like "Client Name", "Budget", etc.)
- **Edit Projects**: Admin can modify any project details
- **Delete Projects**: Admin can remove projects (with confirmation dialog)

#### D. Jira Integration Requirements
**Setup Instructions for Candidates:**
1. Create a free Jira account at atlassian.com
2. Create a project in Jira (can be a simple Kanban board)
3. Generate an API token from Jira
4. Use Jira REST API to connect your application

**Required Jira Functionality:**
- **Auto-Create Jira Board**: When user creates a project in your app, automatically create a corresponding Jira project/board
- **Sync Ticket Data**: Pull ticket information from Jira to display in your dashboard
- **Ticket Status Mapping**: Map Jira statuses to your 4 categories (Closed, In Progress, Not Started, Left)
- **Real-time Updates**: Refresh Jira data at least every hour, or provide a "Refresh" button

### 2. Users Module

#### A. Users List View (Main Users Page)
Create a page showing all users in a table with these columns:
- Profile Picture (placeholder if none)
- Full Name
- Email Address
- Department/Role
- Active Projects (count)
- Join Date
- Status (Active/Inactive)
- Actions (View, Edit, Delete buttons)

**Required Features:**
- Search by name or email
- Filter by department or status
- Sort by any column
- Add New User button

#### B. Individual User Dashboard
When clicking on a user, show their personal dashboard with:

**User Information Section:**
- Profile picture and basic details
- Contact information
- Current project assignments with allocation percentages

**Performance Metrics:**
Display these specific statistics:
- **Last Week**: Number of tickets resolved in the past 7 days
- **Last Month**: Number of tickets resolved in the past 30 days  
- **Last Year**: Number of tickets resolved in the past 365 days
- **All Time**: Total tickets ever resolved

**Current Projects Section:**
- List all projects this user is assigned to
- Show their allocation percentage for each project
- Show their ticket count for each project
- Show current active tickets

**Performance Charts:**
- Monthly ticket completion trend (line graph)
- Project-wise ticket distribution (pie chart or bar chart)

#### C. User Lifecycle Management

**Adding a New User (Required Integrations):**
When an admin adds a new user to the system, your application should:
1. **Create User Record**: Save user details in your database
2. **GitHub Integration**: 
   - Invite user to your GitHub organization
   - Add them to relevant repositories
   - Set appropriate permissions
3. **Jira Integration**:
   - Create Jira user account or invite existing user
   - Add them to relevant Jira projects
   - Assign appropriate Jira permissions
4. **Teams Integration** (if you implement this):
   - Add user to Microsoft Teams
   - Add them to relevant Teams channels

**Removing a User (Required Cleanup):**
When an admin deletes a user, your system must:
1. **Remove from GitHub**: Remove user from organization and repositories
2. **Remove from Jira**: Deactivate user or remove from projects
3. **Remove from Teams**: Remove from Teams organization
4. **Data Cleanup**: 
   - Reassign their open tickets to other users
   - Keep historical data for reporting but mark user as inactive
   - Remove from all project assignments
5. **Send Notifications**: Email relevant project managers about the user removal

### 3. Required API Integrations

#### Jira API Integration
**What you need to implement:**
- Authentication using API tokens
- Create new projects/boards
- Fetch ticket data (issues)
- Get ticket status and assignee information
- Update ticket assignees when users are added to projects

**Sample API Calls to Implement:**
- `GET /rest/api/3/search` - Get tickets/issues
- `POST /rest/api/3/project` - Create new project
- `GET /rest/api/3/project/{projectKey}/statuses` - Get possible statuses

#### GitHub API Integration (Choose GitHub OR Bitbucket)
**Required functionality:**
- Add/remove users from organization
- Create repositories for new projects
- Manage repository permissions
- List user's repositories and contributions

#### Teams Integration (Optional but Preferred)
**If you implement Teams:**
- Add/remove users from Teams
- Create channels for projects
- Send notifications about project updates

### 4. Database Requirements

**Design these database tables at minimum:**
1. **Users Table**: id, name, email, role, department, join_date, status, github_username, jira_account_id
2. **Projects Table**: id, name, description, start_date, end_date, status, github_repo, jira_project_key, created_by
3. **Project_Users Table**: id, project_id, user_id, allocation_percentage, assigned_date
4. **Dynamic_Fields Table**: id, project_id, field_name, field_value (for admin-configurable fields)

**Required Database Operations:**
- CRUD operations for all entities
- Complex queries for dashboard statistics
- Data relationships between projects and users
- Historical data tracking for performance metrics

## Technical Specifications

### Technology Stack
You can use any backend/frontend/database technology of your choice. Consider:
- **Frontend**: React, Vue.js, Angular, or vanilla JavaScript
- **Backend**: Node.js, Python (Django/Flask), Java (Spring), PHP (Laravel), etc.
- **Database**: PostgreSQL, MySQL, MongoDB, etc.
- **Additional tools**: Redis for caching, Docker for containerization

### Required Integrations
1. **Jira API** - For ticket management and board creation
2. **GitHub/Bitbucket API** - For repository management
3. **Microsoft Teams API** - For user management (if applicable)

### Performance Requirements
- Fast loading times for data tables
- Efficient handling of large datasets
- Responsive design for mobile and desktop
- Real-time or near real-time data updates

## Project Structure

```
inma-assessment/
├── README.md (your detailed setup instructions)
├── .env.example
├── backend/
│   ├── (your backend code)
│   ├── models/
│   ├── controllers/
│   ├── routes/
│   ├── services/
│   └── config/
├── frontend/
│   ├── (your frontend code)
│   ├── components/
│   ├── pages/
│   ├── services/
│   └── utils/
├── database/
│   ├── migrations/
│   ├── seeders/
│   └── schema.sql
├── docs/
│   ├── api-documentation.md
│   ├── deployment-guide.md
│   └── user-manual.md
└── docker-compose.yml (optional)
```

## Deliverables

### 1. Complete Web Application
- Single repository with organized folder structure
- Backend API with all required endpoints
- Frontend application with all specified features
- Database schema and migrations

### 2. Documentation
- **Detailed README.md** with:
  - Setup and installation instructions
  - Environment configuration
  - API documentation
  - Deployment instructions
  - Technology choices explanation
- **.env.example** file with all required environment variables
- Code comments and inline documentation

### 3. Integration Setup
- Working Jira integration with API credentials
- GitHub/Bitbucket repository connections
- Teams integration (if implemented)

## What We're Looking For

**You will be judged on your skills to architect the solution, design the pages, and develop the system. Code quality will be taken into account as a major factor in the evaluation.**

This assessment is designed to evaluate your complete software development capabilities across multiple dimensions. We want to see how you approach complex problems, make technical decisions, and deliver a professional solution.

## Evaluation Criteria

### System Architecture (30%)
- **Solution Design**: How well you structure the overall system
- **Technology Choices**: Appropriate selection of frameworks, libraries, and tools
- **Scalability Planning**: Architecture that can grow with business needs
- **Database Design**: Efficient schema design and relationships
- **API Architecture**: RESTful design principles and proper endpoint structure
- **Security Architecture**: Authentication, authorization, and data protection

### Code Quality (25%)
- **Clean Code Practices**: Readable, maintainable, and well-organized code
- **Code Structure**: Proper separation of concerns and modular design
- **Error Handling**: Comprehensive error management and user feedback
- **Performance**: Efficient algorithms and optimized database queries
- **Documentation**: Clear comments and self-documenting code
- **Testing**: Unit tests and integration tests where appropriate

### User Interface & Experience Design (25%)
- **Visual Design**: Professional, clean, and modern interface
- **User Experience**: Intuitive navigation and user workflows
- **Responsive Design**: Works well on desktop, tablet, and mobile devices
- **Accessibility**: Proper semantic HTML and accessibility considerations
- **Data Visualization**: Clear and meaningful charts and statistics
- **Interactive Elements**: Smooth user interactions and feedback

### Technical Implementation (20%)
- **Feature Completeness**: All required functionality implemented and working
- **Integration Quality**: Seamless connection with external APIs (Jira, GitHub, Teams)
- **Data Management**: Proper CRUD operations and data consistency
- **Real-time Features**: Live updates and dynamic content
- **Deployment Ready**: Production-ready configuration and setup

## Timeline

- **Assessment Duration**: [25th June 2025 - 1st July 2025]
- **Submission Deadline**: [1st July 2025]

## Submission Guidelines

1. Ensure your repository is complete with all deliverables
2. Create a comprehensive README with setup instructions
3. Include a brief video demo (5-10 minutes) showcasing key features
4. Send the repository link to [INSERT EMAIL]
5. Be prepared for a technical discussion about your implementation

## Support & Questions

If you have questions about requirements or need clarification:
- **Technical Questions**: aashijit@indpro.se
- **General Questions**: hrd@indpro.se

## Important Notes

- **Originality**: All code must be your own work
- **External Libraries**: You may use any open-source libraries and frameworks
- **AI Tools**: Please mention if you used any AI assistance in your README
- **Testing**: Include unit tests where appropriate
- **Security**: Implement proper authentication and authorization

## Success Tips

1. **Start with MVP**: Build core functionality first, then add enhancements
2. **Focus on UX**: Create intuitive and user-friendly interfaces  
3. **Document Everything**: Clear documentation is highly valued
4. **Test Thoroughly**: Ensure all features work as expected
5. **Think Scalability**: Design with future growth in mind

Good luck, and we look forward to seeing your innovative solution for Indpro Manager!

---

**Remember**: This assessment is an opportunity to showcase your full-stack development skills, problem-solving ability, and understanding of business requirements. Quality over quantity - a well-implemented core solution is better than a half-finished complex one.