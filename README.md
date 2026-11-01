# Task 3: Task Automation with Python Scripts

## Project title
**JPG File Organizer – Automatic File Moving Script**

## Project description
This Python project automates a repetitive file-management task. It finds all `.jpg` files in a source folder and moves them into a destination folder. The user enters both folder paths when the program runs.

## Selected assignment idea
Move all `.jpg` files from a folder to a new folder.

## Features
- Takes source and destination folder paths from the user.
- Finds `.jpg` files (case-insensitive extension check).
- Creates the destination folder if it does not already exist.
- Moves files using Python's `shutil` module.
- Avoids overwriting files if a filename already exists by adding a number.
- Displays the number of files moved.
- Handles missing folders and file-operation errors.

## Concepts used
- `pathlib` for working with folder and file paths.
- `os`-style file-system operations through Python's path utilities.
- `shutil.move()` for moving files.
- Functions, loops, conditional statements, and exception handling.

## Requirements
- Python 3.8 or newer.
- No external libraries are required.

## How to run
1. Extract the ZIP file.
2. Open the project folder in VS Code.
3. Open the terminal.
4. Run:

   ```bash
   python jpg_file_organizer.py
   ```

5. Enter the full path of the folder containing JPG files.
6. Enter the full path of the destination folder.

### Example (Windows)

Source folder:
```text
C:\Users\YourName\Pictures\Unsorted
```

Destination folder:
```text
C:\Users\YourName\Pictures\JPG_Files
```

The script moves `.jpg` files from `Unsorted` to `JPG_Files`. Replace `YourName` with your Windows account folder name.

## Important notes
- Test the script with a copy of sample files first.
- The script moves files; it does not make copies.
- Only files directly inside the source folder are processed. It does not scan subfolders.
- Existing destination files are not overwritten.
