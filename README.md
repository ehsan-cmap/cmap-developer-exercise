# Timesheet System

## Objective  
Design and implement a timesheet system where users can enter timesheet entries and save them to an in-memory database. The system must have the ability to download the entries as a CSV file. Unit tests should be included to ensure the robustness of the system.

## Acceptance Criteria

1. **Timesheet Entry:**
   - Users can enter the following details: user name, date, project name, description of tasks, and hours worked.
   - **Sample Data Form:**

| User Name      | Date       | Project       | Description of Tasks      | Hours Worked |
|----------------|------------|---------------|---------------------------|--------------|
| John Smith     | 22/10/2014 | Project Alpha | Developed new feature X   | 4            |

2. **In-Memory Database:**
   - Timesheet entries should be stored in an in-memory database to demonstrate persistence.
   - If a user has added multiple timesheet entries on the same day, the total hours for that day should be stored, to be made available within the CSV download.

3. **Download to CSV:**
   - Users can export the timesheet data to a CSV file.
   - A column must be added to show the total hours a user has worked if they have multiple timesheet entries on the same day.
   - **Sample Data Table:**

| User Name      | Date       | Project       | Description of Tasks      | Hours Worked | Total Hours for the Day |
|----------------|------------|---------------|---------------------------|--------------|-------------------------|
| John Smith     | 22/10/2014 | Project Alpha | Developed new feature X   | 4            | 8                       |
| John Smith     | 22/10/2014 | Project Beta  | Fixed bugs in module Y    | 4            | 8                       |
| Jane Doe       | 22/10/2014 | Project Gamma | Conducted user testing    | 6            | 6                       |

4. **Unit Testing:**
   - Unit tests should cover the core functionalities: submitting timesheet entries, CSV data structure, and downloading to CSV.

## Constraints

- An in-memory database should be used for persistence so that we can review a working and complete application.
- We'd like to see the backend implemented in C#. For simplicity, you could opt for ASP.NET MVC.

## Guidance

- Making small commits and showing your commit history is recommended so that we can see your approach. For example, if you're using Test Driven Development then show us.
- Keep it simple and take as much time as you need, the aim is to demonstrate your approach.
- You do not need to deploy the application.
- There is no need to fork our repo. Submit a link to your GitHub repository privately.
