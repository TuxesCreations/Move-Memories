# Moving Memories

**Date:** June 23, 2024  
**File Name:** Moving Memories  
**Developed in:** AppleScript  
**Version:** 1.0  
**Made with Love by:** TuxesCreations and Aurora  
**Contact:** TuxesCreations@example.com

---

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Requirements](#requirements)
4. [Usage Instructions](#usage-instructions)
5. [Debugging and Logging](#debugging-and-logging)
6. [Best Practices](#best-practices)
7. [Known Issues](#known-issues)
8. [Future Improvements](#future-improvements)
9. [Contact Information](#contact-information)

---

## Introduction

**Moving Memories** is an AppleScript designed to help you organize and move files from a source folder to a destination folder. It ensures that files are uniquely named by appending the parent folder name and a random suffix to the filenames. It also handles `.json` files by deleting them and removes empty folders after processing.

---

## Features

- **Recursive Folder Processing**: Processes all files and subfolders within the specified source folder.
- **Unique Filename Generation**: Appends the parent folder name and a random suffix to filenames to avoid duplicates.
- **JSON File Handling**: Deletes any `.json` files encountered during processing.
- **Empty Folder Removal**: Deletes empty folders after processing all items within them.
- **Verbose Logging**: Logs all actions and errors to a file on the desktop if logging is enabled.
- **Debug Mode**: Provides detailed dialogs for actions taken if debug mode is enabled.

---

## Requirements

- **AppleScript**: This script is developed using AppleScript.
- **OpenSSL**: The script uses the `openssl` command to generate random suffixes. Ensure OpenSSL is installed on your system.

---

## Usage Instructions

1. **Download and Open**: Download the script file and open it in the Script Editor on your Mac.
2. **Set Debug Flags**: Optionally, set the `dialogDebugFlag` and `logDebugFlag` properties to `true` to enable dialogs and logging, respectively.
3. **Run the Script**: Click the "Run" button in the Script Editor.
4. **Select Folders**: You will be prompted to choose the source and destination folders.
5. **Processing**: The script will process the source folder, moving files to the destination folder and handling JSON files and empty folders as specified.
6. **Summary**: After processing, a summary dialog will display the total number of files found, moved, and JSON files deleted.

---

## Debugging and Logging

- **Enable Debug Mode**: Set `dialogDebugFlag` to `true` to enable detailed dialogs for each action.
- **Enable Logging**: Set `logDebugFlag` to `true` to log all actions and errors to a file on the desktop (`file_processing_log.txt`).
- **Log File Location**: The log file is saved to your desktop as `file_processing_log.txt`.

---

## Best Practices

- **Back Up Data**: Always back up your data before running the script to prevent any accidental data loss.
- **Test with Sample Data**: Test the script with a small set of sample data to ensure it performs as expected before running it on a larger dataset.
- **Review Logs**: If logging is enabled, review the log file to verify that all actions have been performed correctly and to troubleshoot any issues.
- **Keep Dependencies Updated**: Ensure OpenSSL is installed and up to date on your system for generating random suffixes.

---

## Known Issues

- **File Name Collisions**: In rare cases, even with a random suffix, there might be filename collisions if the same random suffix is generated multiple times. This script does not handle such collisions.
- **Path Length Limitations**: Very long file paths might cause issues during processing due to system path length limitations.

---

## Future Improvements

- **Collision Handling**: Implement additional checks to handle rare filename collisions even with random suffixes.
- **Error Recovery**: Improve error handling to recover from errors and continue processing remaining files.
- **Performance Optimization**: Optimize the script to handle large datasets more efficiently.

---

## Contact Information

For any questions, issues, or feature requests, please contact us at:  
**Email:** hello@tuxescreations.com

---

Thank you for using Moving Memories! We hope this script helps you organize your files efficiently.

---