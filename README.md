# Amateur Radio Call Manager

Desktop application built for an amateur radio operator to register, edit, delete and export radio call records.

The project started from a real request from my college professor, Virgilio Cesar Leandro. The goal was to replace spreadsheet-only tracking with a small local app using a graphical interface and SQLite.

## What It Shows

- Python desktop UI with PyQt5.
- SQLite persistence.
- CRUD operations for call records.
- Table refresh after inserts, updates and deletes.
- Export to Excel for sharing and backup.

## Stack

- Python
- PyQt5
- SQLite
- pandas
- openpyxl
- xlwt

## Project Structure

```text
amateur_radiocall_manager/
  main.py
  *.ui
  ui_*.py
  Gerenciador.spec
  requirements.txt
  README.md
```

## Setup

```bash
python -m venv .venv
.venv/Scripts/activate
pip install -r requirements.txt
python main.py
```

The local SQLite database is created at runtime and is intentionally ignored by Git.

## Features

- Add call records with date, time, frequency and notes.
- Edit existing records.
- Delete records by ID.
- Export the table to an Excel file.
- Keep the interface table updated after changes.

## Screenshots

![Main screen](https://user-images.githubusercontent.com/113928099/228587507-17bb354d-e412-49f4-812c-dd4de65f9b79.png)
![Insert screen](https://user-images.githubusercontent.com/113928099/228587599-5790fa37-e634-43b4-9731-7a41c96b9417.png)
![Table screen](https://user-images.githubusercontent.com/113928099/228587941-b570c1ff-aeab-4593-846f-9f12041605b1.png)

## Next Improvements

- Package the app with a repeatable build command.
- Add stronger form validation.
- Add automated tests for database operations.
- Improve UI spacing and error messages.

