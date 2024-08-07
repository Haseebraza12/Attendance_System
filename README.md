Attendance Platform UI Design Document
1. Introduction
The Attendance Platform is a user interface application built using Python and PyQt6. The application allows a lecturer or administrator to manually mark students as either present or absent and export this data as a text file. It also displays student details and photos in a dock widget. This document details the design decisions made for the User Interface (UI) of the Attendance Platform.
2. User Interface Design
2.1 Main Window Layout
2.1.1 Layout and Containers
Main Widget: The central container for all UI elements, set to a QVBoxLayout to stack child widgets vertically.
Main Layout: Contains the student table and the button layout. This vertical layout ensures that the table occupies most of the window space, with the buttons conveniently placed below it.
2.1.2 Student Table
QTableWidget: Displays the list of students with columns for student number, name, programme, and attendance status. The table supports row selection and single selection mode to focus on one student at a time.
Headers: 'Student Number', 'Name', 'Programme', 'Attendance'.
2.2 Buttons
2.2.1 Set Date Button
Functionality: Opens a dialog to select a different date for attendance. The selected date updates the main window title.
Animation: Animated to enhance user interaction.
2.2.2 Mark All Present Button
Functionality: Marks all students as present.
Animation: Animated to enhance user interaction.
2.2.3 Mark All Absent Button
Functionality: Marks all students as absent.
Animation: Animated to enhance user interaction.
2.2.4 Reset Attendance Button
Functionality: Clears attendance status for all students.
Animation: Animated to enhance user interaction.
2.2.5 Export Attendance Button
Functionality: Exports attendance data to a text file named with the current date.
Animation: Animated to enhance user interaction.
2.3 Dock Widget
2.3.1 Layout and Containers
QDockWidget: Displays detailed information about the selected student, including a photo.
Vertical Layout: Ensures a clean and organized display of student details and photo.
2.3.2 Student Details
QLabel: Displays student number, name, and programme.
QLabel for Photo: Displays the student's photo, scaled to fit within a fixed size of 150x150 pixels.
2.3.3 Edit Button
Functionality: Opens a dialog to edit student details. Updates the table and CSV file upon confirmation.
Animation: Animated to enhance user interaction.
2.4 Styling and Customization
2.4.1 Gradient Background
QMainWindow: Styled with a linear gradient background for visual appeal. The gradient transitions from a light purple to white.
2.4.2 Buttons
QPushButton: Styled with custom colors, padding, and border radius. Buttons change color on hover to provide feedback.
2.4.3 Labels
QLabel: Styled for readability, with a font size of 14px and a neutral color scheme.
3. Additional Features
3.1 Responsive Design
The UI components are designed to be responsive, adjusting to different window sizes to ensure usability on various screen resolutions.
3.2 Animation Enhancements
Buttons include animations to improve user experience by providing visual feedback and making interactions more engaging.
4. Conclusion
The Attendance Platform UI is designed with usability and visual appeal in mind. By organizing elements logically and applying consistent styling, the application aims to provide a seamless experience for lecturers and administrators managing student attendance. The detailed documentation of design decisions ensures that the UI is well-understood and can be maintained or extended in the future.

