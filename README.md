# LinguaLearn

A Flutter mobile app for learning languages in small, structured steps.

## Project Vision
Help people who want to learn English, Arabic, and other languages by giving them clear programs organized by level, with progress tracking. Give teachers and institutes a simple admin dashboard to manage programs and lessons.

## Objectives
- Give learners a clear path from Beginner to Advanced in each language.
- Let learners browse, enroll in programs, and track progress.
- Let admins add, edit, and delete programs and lessons, and view learners.
- Plan the UI and navigation flow before coding (Week 1), then build the screens in Flutter (Week 2).

## Target Users
| User | Description |
|------|-------------|
| Learner | Students and professionals who want to learn a language |
| Admin | Teacher or institute staff who manage programs and lessons |

## Key Features
**Learner:** sign up / login, browse and search programs, program details with lesson list, enroll, lessons (vocabulary and short quiz), progress tracking, profile.

**Admin:** login, dashboard, add / edit / delete programs and lessons, view learners list.

## Navigation Flow
```
Login
 |-- Learner --> Home <--> Programs <--> Profile   (bottom navigation)
 |                |           |
 |                +--> Program Details --> Enroll
 |
 |-- Admin --> Admin Dashboard --> Add / Edit Program
 |
 +-- Sign up --> Home
```

| From | Action | To |
|------|--------|----|
| Login | Login as Learner | Home |
| Login | Login as Admin | Admin Dashboard |
| Home | Tap program or Continue learning | Program Details |
| Programs | Tap View | Program Details |
| Program Details | Enroll Now | Home (enrolled) |
| Profile / Dashboard | Logout | Login |

## Planned Folder Structure
```
lib/
  main.dart
  screens/    (login, home, program listing, program details, profile, admin dashboard)
  widgets/    (reusable UI parts)
  models/     (Program, Lesson, User)
  utils/      (theme, colors, routes)
assets/
```

## Getting Started
```bash
git clone https://github.com/<username>/lingualearn.git
cd lingualearn
flutter pub get
flutter run
```

## Future Scope
Audio pronunciation, more languages, certificates, and daily reminder notifications.

## Status
Week 1: proposal, wireframes, and repository setup completed.
