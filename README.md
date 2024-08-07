
# Attendance Platform

## Overview

The Attendance Platform is a desktop application built using Python and PyQt6, designed to help lecturers and administrators manage student attendance efficiently. The application provides functionalities to mark attendance, view student details, and export attendance data.

## Features

1. **User Interface**: A responsive and intuitive UI for easy navigation and usability.
2. **Student Table**: Displays student information including student number, name, programme, and attendance status.
3. **Set Date**: Allows users to set the attendance date using a calendar dialog.
4. **Mark All Present/Absent**: Provides buttons to mark all students as either present or absent with a single click.
5. **Reset Attendance**: Clears all attendance records to start fresh.
6. **Export Attendance**: Exports the attendance data to a text file named with the current date.
7. **Dock Widget**: Displays detailed information and photo of the selected student.
8. **Edit Student Details**: Allows users to edit student details and updates the CSV file accordingly.
9. **Styling and Animations**: Custom styling and animations for a better user experience.

## Installation

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/attendance-platform.git
    cd attendance-platform
    ```

2. **Install dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

3. **Ensure your working directory contains the following files**:
    - `attendance_platform.py` (main application file)
    - `students.csv` (CSV file with student information)
    - `images/` (folder containing student photos, named as per student numbers in the CSV)

## Usage

1. **Run the application**:
    ```sh
    python attendance_platform.py
    ```

2. **User Interface**:
    - **Student Table**: Displays student information. Select a student to view details and photo in the dock widget.
    - **Set Date**: Click the "Set Date" button to open a calendar dialog and select a date.
    - **Mark All Present/Absent**: Use these buttons to mark the attendance status of all students.
    - **Reset Attendance**: Clears all attendance records.
    - **Export Attendance**: Saves the attendance data to a text file.
    - **Edit Student Details**: Click the "Edit" button in the dock widget to edit student details.

3. **Dock Widget**:
    - Displays detailed information and photo of the selected student.
    - Use the "Edit" button to update student details.

## File Structure

```
attendance-platform/
│
├── attendance_platform.py    # Main application file
├── students.csv              # CSV file with student information
├── images/                   # Folder containing student photos
│   ├── student1.png
│   ├── student2.png


## CSV File Structure

The `students.csv` file should have the following structure:
```
Student Number, Name, Programme, Image Path
1, John Doe, Computer Science, images/student1.png
2, Jane Smith, Information Technology, images/student2.png
...
```

##
