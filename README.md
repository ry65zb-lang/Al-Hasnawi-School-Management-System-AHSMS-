from pathlib import Path
import pypandoc

text = r"""# Al Hassnawi Global Educational App
## Project Progress Tracker

Last Update: 2026-07-05

## Project Status
- Name: Al Hassnawi Global Educational App
- Status: In Development
- Estimated Progress: 15%

## Completed
### Visual Identity
- New project name adopted.
- New logo approved.
- Visual identity direction defined.

### Project Architecture
- Flutter folder structure planned.
- main.dart entry point planned.
- app.dart structure planned.
- Material 3 selected.
- Initial dashboard architecture designed.

### Models
- Student model.
- Teacher model.
- User model.
- UserRole enum.

### Services
- Initial AuthService.
- Initial StudentService.

### Database Design
Initial schema designed for:
- Users
- Students
- Teachers
- Classes
- Subjects
- Grades
- Attendance
- Notifications

## Current Task
### Student Management Module
Remaining:
- Students list screen
- Add student screen
- Edit student screen
- Delete student
- Search
- Supabase integration
- Excel import/export
- PDF export

## Upcoming Modules
1. Student Management
2. Teacher Management
3. Classes & Sections
4. Subjects
5. Timetable
6. Grades
7. Attendance
8. Parents
9. Finance
10. Reports
11. Notifications
12. Settings
13. Users & Permissions
14. Backup
15. Full Supabase Integration
16. Testing & Bug Fixes
17. Android APK/AAB
18. Web Deployment
19. Version 1.0 Release

## Technologies
- Flutter
- Dart
- Supabase
- Riverpod
- GoRouter
- Material 3
- PDF Export
- Excel Import/Export

## Resume Instructions
When continuing the project:
1. Open this file.
2. Check "Current Task".
3. Complete it.
4. Move it to "Completed".
5. Continue with the next module.
"""
out="/mnt/data/PROJECT_PROGRESS.md"
pypandoc.convert_text(text,"md",format="md",outputfile=out,extra_args=["--standalone"])
print(out)
