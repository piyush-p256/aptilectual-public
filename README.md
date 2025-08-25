# Aptilectual

Aptilectual is a Django web application designed to help users practice and improve their aptitude skills by solving daily problems. Features include user registration, login, solving daily problems, viewing leaderboards, and reviewing past problems.

## Table of Contents

- [Features](#features)
- [Endpoints](#endpoints)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [License](#license)

## Features

### For Students

- **Daily Problems:** Access daily aptitude questions to improve skills.
- **Leaderboards:** View daily and monthly leaderboards to track performance.
- **Placement Applications:** Apply for placement drives and view eligibility.
- **Search Functionality:** Search for problems, companies, and placement drives.
- **Custom Email Notifications:** Receive personalized emails regarding placement drives and updates.

### For Cell Admins

- **Placement Drive Management:** Create and manage placement drives.
- **Student Eligibility:** Filter students based on eligibility criteria.
- **Custom Email Sending:** Send personalized emails to selected students with attachments.
- **Company Problem Management:** Add and manage company-specific problems.
- **Student Performance Tracking:** View daily attempted questions and leaderboards.

### For Super Admins

- **User Management:** Manage student and admin accounts.
- **Company Management:** Add and manage companies participating in placement drives.
- **Advanced Filters:** Filter students based on branches, batches, and registration status.
- **Custom Email Templates:** Create and send custom email templates.

## Endpoints

### Student Endpoints

- `/daily-problems/`: View daily aptitude questions.
- `/leaderboard/daily/`: View daily leaderboard.
- `/leaderboard/monthly/`: View monthly leaderboard.
- `/placement-application/`: Apply for placement drives.

### Admin Endpoints

- `/placement-drive/create/`: Create a new placement drive.
- `/placement-drive/manage/`: Manage existing placement drives.
- `/email/send/`: Send custom emails to students.
- `/company-problems/add/`: Add company-specific problems.

### Super Admin Endpoints

- `/user/manage/`: Manage user accounts.
- `/company/manage/`: Manage company details.
- `/email/templates/`: Create and manage email templates.

## Installation

### Prerequisites

- Python 3.6+
- Django 3.0+
- SQLite (default database)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/aptitude-platform.git
   cd aptitude-platform
   ```
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: `venv\Scripts\activate`
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Apply migrations:
   ```bash
   python manage.py migrate
   ```
5. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```
6. Run the development server:
   ```bash
   python manage.py runserver
   ```
7. Open the app in your browser: `http://127.0.0.1:8000/`.

## Usage

- **User Authentication**: Register, log in, and manage your profile.
- **Daily Problems**: Solve problems during the specified window (17:00 to 22:00).
- **Leaderboards**: View daily and monthly leaderboards.
- **Past Problems**: Review previous problems and answers.

## Project Structure

```
aptitude_platform/
├── aptitude/
│   ├── models.py
│   ├── views.py
│   ├── templates/
│   └── ...
├── aptitude_platform/
│   ├── settings.py
│   └── urls.py
├── manage.py
├── requirements.txt
└── README.md
```


## Note

This is a private repository. If you are a recruiter and wish to view the code, please contact me at [piyushpatel2562004@gmail.com](mailto:piyushpatel2562004@gmail.com).
