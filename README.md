                                                    OBITUARY PLATFORM
Project Documentation: Obituary Platform

1. Overview
Project Name: Obituary Platform

Description: A web application for submitting, viewing, editing, and deleting obituaries.

Technologies Used: Python (Flask), SQLAlchemy, SQLite, HTML, CSS, Jinja2 templates.

3. Project Structure
File Structure:

app.py: Main Flask application file containing routes and database configuration.

models.py: Defines SQLAlchemy model (Obituary) for database interactions.

templates/: Directory containing HTML templates.

static/: Directory for static files (CSS, JavaScript).

4. Features
Submission:

Users can submit obituaries with fields for name, dates, content, and author.

Generates a unique slug for each obituary based on the name.

Viewing:

Displays a list of obituaries with search filters for name, month, and year.

Table format with columns for name, dates, content, author, and submission date.

Editing:

Allows authorized users to edit obituaries using a dedicated edit form.

Updates database records with new information.

Deleting:

Provides a mechanism to delete obituaries from the database.

Confirmation prompt for deletion action.

4. Code Details
app.py

Flask routes for rendering templates (index, submit_obituary, view_obituaries).

Database setup using SQLAlchemy (Obituary model).

Functions for generating slugs (generate_slug) and handling form submissions.

models.py

Defines the Obituary model with fields (id, name, date_of_birth, date_of_death, content, author, submission_date, slug).

Manages database interactions and relationships.

Templates (templates/)

HTML Templates:
obituary_form.html: Form for submitting new obituaries.

view_obituaries.html: Displays a list of obituaries with search filters.

edit_obituary.html: Form for editing existing obituaries.


Static Files (static/)

CSS (style.css): Styles the web application for consistent design and responsiveness.

JavaScript (form_validation.js): Client-side validation for form inputs.

5. Installation and Setup

Requirements:

Python 3.x

Flask

SQLAlchemy

Setup Instructions:

Clone the repository  

                https://github.com/Kungu-Prince/Obituary-Platform.git
                
Install dependencies 

               pip install -r requirements.txt
               
Configure the database URI in app.py.
Run the application 

               flask run
               
6. Usage
Submitting an Obituary:

Access the homepage (/).

Fill out the submission form and submit.

Viewing Obituaries:

Navigate to /view_obituaries.

Use search filters to refine results.

Editing or Deleting:

Edit: Click on "Edit" next to an obituary, make changes, and submit.

Delete: Click on "Delete" and confirm the action.

7. Future Enhancements
Implement user authentication for editing and deleting obituaries.

Add image uploads for obituaries.

Enhance search functionality with additional filters.

9. Contributors
Developer: Prince Kung'u

11. License
This project is licensed under MIT License.
