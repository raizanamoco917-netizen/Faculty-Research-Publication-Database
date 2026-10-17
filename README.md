# Faculty Research & Publication Database

**Project Name:** Faculty Research & Publication Database  
**Developer:** Raiza D. Namoco  
**Project Type:** Academic Research Database Management System

## 1. Project Description

The Faculty Research & Publication Database is a database management system designed to organize and manage faculty information, research projects, research areas, publications, journals, and researcher participation in academic institutions.

The system uses Google Sheets to store and organize data and AppSheet to provide a user-friendly application for viewing, adding, updating, and managing records. GitHub is used to document the project, its purpose, features, and instructions.

This project aims to make faculty research information easier to access, maintain, and monitor.

## 2. Project Objectives

The objectives of this project are to:

- Organize faculty and department information.
- Manage research projects and their research areas.
- Record academic publications and journal information.
- Track faculty members participating in research projects.
- Maintain relationships between researchers, research projects, and publications.
- Reduce duplicate and inconsistent data through proper database design.
- Provide an accessible application for managing research records.
- Support the monitoring of faculty research and publication activities.

## 3. Main Features

- **Faculty Management** – Store faculty names, email addresses, positions, and department assignments.
- **Department Management** – Organize faculty members according to their departments.
- **Research Management** – Record research titles, research areas, statuses, and dates.
- **Research Area Management** – Classify research projects according to their areas of study.
- **Researcher Management** – Record faculty participation in research projects and their roles.
- **Publication Management** – Store publication titles, publication dates, DOI information, and related research.
- **Journal Management** – Maintain journal names, ISSN numbers, and publisher information.
- **Data Relationships** – Connect related records through primary keys, foreign keys, and references.
- **Record Management** – Use AppSheet forms and views to add, display, and update records when configured.
- **Research Monitoring** – Support reviewing research and publication records.

## 4. Technologies Used

### AppSheet
AppSheet is used to build the application interface. It allows users to interact with the database through forms, tables, detail views, and other configured views without requiring a traditional application codebase.

### Google Sheets
Google Sheets serves as the spreadsheet-based data source for storing the database records and organizing the project's tables.

### GitHub
GitHub is used to store the project's README documentation and other project files, making the project information easier to maintain and share.

## 5. Database Structure

The database consists of seven main tables.

| Table | Description |
|---|---|
| Department | Stores department identification and department names. |
| Faculty | Stores faculty member information and department assignments. |
| Research_Area | Stores research area identifiers and area names. |
| Research | Stores research titles, research areas, statuses, and research dates. |
| Researcher | Connects faculty members to research projects and records their roles. |
| Publication | Stores publication titles, dates, DOI information, and related research and journals. |
| Journal | Stores journal names, ISSN numbers, and publisher information. |

### Important Relationships

- One department can have multiple faculty members.
- One research area can be associated with multiple research projects.
- One faculty member can participate in multiple research projects.
- One research project can involve multiple faculty members.
- One research project can have multiple publications.
- One journal can be associated with multiple publications.

The **Researcher** table serves as the linking table between Faculty and Research, allowing the database to represent their many-to-many relationship.

## 6. Database Keys and Data Integrity

The database uses identifiers to distinguish records and connect related tables.

- **Primary Key (PK):** Uniquely identifies each record in a table.
- **Foreign Key (FK):** References a related record in another table.
- **Reference (Ref):** In AppSheet, connects a column to a record in another table.
- **Data Validation:** Helps ensure that users enter appropriate values into the database.

Examples of identifiers include `Faculty_ID`, `Department_ID`, `Research_ID`, `Publication_ID`, and `Journal_ID`.

## 7. How to Use the Application

### Step 1: Open the Application
Open the AppSheet application using the application link provided by the developer.

### Step 2: View the Available Sections
Navigate through the configured views to access faculty, departments, research areas, research projects, researchers, publications, and journals.

### Step 3: Add a Record
Open the appropriate section, select the add or new-record option, fill in the required fields, and save the form.

### Step 4: Update a Record
Open an existing record, select the edit option if available, modify the necessary information, and save the changes.

### Step 5: Review Related Information
Use the configured references and related-record views to examine connections between faculty members, departments, research projects, and publications.

### Step 6: Check the Data
Confirm that records have the correct identifiers and that related records exist before saving or relying on the information.

*Note: The exact menu names, available actions, and navigation depend on the current AppSheet configuration and user permissions.*

## 8. Database Design and Normalization

The database structure is intended to organize information into related tables instead of storing all information in one large table.

### First Normal Form (1NF)
Each field should contain a single value, and each record should be uniquely identifiable.

### Second Normal Form (2NF)
The database should satisfy 1NF, and every non-key attribute should depend on the whole primary key. This is particularly important when a table uses a composite primary key.

Normalization helps reduce unnecessary duplication and improve data consistency.

## 9. Project Benefits

- Provides an organized location for faculty research information.
- Makes research and publication records easier to manage.
- Helps identify faculty participation in research projects.
- Improves consistency through related database tables.
- Supports more convenient access to academic research information.
- Provides a foundation for reviewing research and publication activity.

## 10. Project Limitations

- The application depends on the configured AppSheet application and its connected data source.
- Data accuracy depends on the information entered by authorized users.
- Available functions depend on the implemented views, actions, validation rules, and access permissions.
- Dashboard summaries, automated notifications, advanced reports, and security controls are available only if they have been configured.

## 11. Future Improvements

Possible future improvements include:

- Adding a research and publication dashboard.
- Creating search and filtering tools.
- Adding publication and research-status summaries.
- Improving input validation and duplicate prevention.
- Adding automated notifications for research updates.
- Improving user access controls and data security.
- Providing exportable reports for academic monitoring.

These improvements are suggestions and should not be considered implemented unless they are available in the current application.

## 12. Project Links

- **AppSheet Application:** [Open the Faculty Research & Publication Database](https://www.appsheet.com/Template/AppDef?appName=FacultyandPublication-756053880&utm_source=share_app_link)
- **GitHub Repository:** Add your GitHub repository URL here.
- **Google Sheets Data Source:** Add the appropriate Google Sheets link here if you want to share it and have permission to do so.

## 13. Conclusion

The Faculty Research & Publication Database provides a structured approach to managing faculty information, research projects, researcher participation, academic publications, and journal records. By combining AppSheet, Google Sheets, and GitHub, the project demonstrates how a relational database design can support the organization and management of academic research information.

The project also applies fundamental database concepts, including primary keys, foreign keys, relationships, and normalization, to help maintain consistent and organized records.
