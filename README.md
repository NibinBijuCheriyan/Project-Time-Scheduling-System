# Project Scheduler

A simple yet powerful Python-based project scheduling system that helps you keep track of project deadlines and manage your project timeline effectively.

## Features

- **Project Management**
  - Create new projects with deadlines and descriptions
  - Remove existing projects
  - Mark projects as completed
  - Persistent storage using JSON

- **Deadline Tracking**
  - Set and monitor project deadlines
  - View upcoming deadlines within a specified timeframe
  - Calculate remaining days for each project
  - Prevention of past dates for new projects

- **Project Overview**
  - Display all projects with their current status
  - Sort projects by deadline
  - View detailed project information

## Requirements

- Python 3.x
- No additional external dependencies required

## Installation

1. Clone or download the project files to your local machine
2. Ensure you have Python 3.x installed
3. No additional package installation is required

## Usage

1. Run the program:
```bash
python project_scheduler.py
```

2. Use the menu-driven interface to:
   - Add new projects (Option 1)
   - Remove projects (Option 2)
   - Mark projects as completed (Option 3)
   - View upcoming deadlines (Option 4)
   - View all projects (Option 5)
   - Exit the program (Option 6)

### Adding a Project

When adding a project, you'll need to provide:
- Project name (required)
- Deadline in YYYY-MM-DD format (required)
- Project description (optional)

Example:
```
Enter project name: Website Redesign
Enter deadline (YYYY-MM-DD): 2025-03-15
Enter project description (optional): Complete company website overhaul
```

### Viewing Projects

You can view projects in two ways:
1. View upcoming deadlines within a specified number of days
2. View all projects with their complete details

## Data Storage

- All project data is automatically saved to `projects.json` in the same directory
- Data persists between program sessions
- The JSON file is automatically created on first use

## Error Handling

The system includes handling for:
- Invalid date formats
- Past dates for new projects
- Duplicate project names
- Invalid menu selections

## File Structure

```
project_scheduler/
│
├── project_scheduler.py    # Main program file
└── projects.json          # Data storage file (auto-generated)
```

## Classes and Methods

### Project Class
- Stores individual project information
- Properties: name, deadline, description, completed status

### ProjectScheduler Class
- Main class handling all scheduling operations
- Methods:
  - `add_project()`: Add a new project
  - `remove_project()`: Remove an existing project
  - `mark_completed()`: Mark a project as completed
  - `get_upcoming_deadlines()`: Get projects due within specified days
  - `display_all_projects()`: Show all project details
  - `load_projects()`: Load projects from JSON file
  - `save_projects()`: Save projects to JSON file

## Contributing

Feel free to fork this project and submit improvements or bug fixes via pull requests.

## License

This project is open source and available under the MIT License.
