# Codebase Line Counter

A Python script that counts non-empty lines of code per programming language in a project directory. It respects `.gitignore` rules, excludes common lock and build files/directories, and shows incremental progress during scanning.

## Features

-   Detects languages based on file extensions
-   Skips files and directories excluded by `.gitignore` and predefined lists
-   Counts only non-empty lines
-   Displays progress every N files processed (default 50)
-   Provides a summary report sorted by total lines per language

## Usage

1. Clone or download this repository.
2. Run the script from the root of your project:

```bash
python program.py
```

## Example Output

```
Processed 50 files...
Processed 100 files...
Processed 150 files...

TypeScript      3370 lines
    2340 lines  ./web/app.tsx
    1030 lines  ./web/store.ts

Python          2344 lines
    1234 lines  ./src/main.py
    1110 lines  ./src/utils/helpers.py

JavaScript      1440 lines
     890 lines  ./web/app.js
     450 lines  ./web/components/button.jsx

```
