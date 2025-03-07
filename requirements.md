
```
# Requirements for Crossref API Tool
# Last Updated: March 06, 2025

This file lists the software dependencies required to run the Crossref API Tool, a Bash script for retrieving scientific article information from the Crossref REST API. Before using the script, ensure the following packages are installed on your Linux system.

## Required Software

1. **curl**
   - Purpose: Used to make HTTP requests to the Crossref API.
   - Installation (Ubuntu/Debian):
     ```
     sudo apt update
     sudo apt install curl
     ```
   - Installation (Fedora):
     ```
     sudo dnf install curl
     ```
   - Installation (Arch Linux):
     ```
     sudo pacman -S curl
     ```

2. **jq**
   - Purpose: A lightweight command-line JSON processor used to parse API responses.
   - Installation (Ubuntu/Debian):
     ```
     sudo apt update
     sudo apt install jq
     ```
   - Installation (Fedora):
     ```
     sudo dnf install jq
     ```
   - Installation (Arch Linux):
     ```
     sudo pacman -S jq
     ```

3. **rofi**
   - Purpose: A window switcher and application launcher used for interactive menus in the script.
   - Installation (Ubuntu/Debian):
     ```
     sudo apt update
     sudo apt install rofi
     ```
   - Installation (Fedora):
     ```
     sudo dnf install rofi
     ```
   - Installation (Arch Linux):
     ```
     sudo pacman -S rofi
     ```

4. **xclip**
   - Purpose: Allows copying search results to the clipboard.
   - Installation (Ubuntu/Debian):
     ```
     sudo apt update
     sudo apt install xclip
     ```
   - Installation (Fedora):
     ```
     sudo dnf install xclip
     ```
   - Installation (Arch Linux):
     ```
     sudo pacman -S xclip
     ```

## Verification
After installing, verify that each tool is available by running the following commands in your terminal:
```
curl --version
jq --version
rofi --version
xclip -version
```
If any command fails, recheck the installation steps for that package.

## Notes
- This script is designed for Linux systems with a Bash shell.
- Ensure you have an active internet connection, as the script interacts with the Crossref API over the web.
- No additional configuration files or API keys are required for the Crossref API, as it provides open access for basic queries.

## How to Run the Script
1. Place the following files in the same directory:
   - crossref_tool.sh
   - functions.sh
   - config.rasi
   - requirements.txt (this file)
2. Make the scripts executable:
   ```
   chmod +x crossref_tool.sh functions.sh
   ```
3. Run the main script:
   ```
   ./crossref_tool.sh
   ```

If you encounter issues, ensure all dependencies are installed and refer to the terminal output for error messages.

If the search input is entered in the terminal instead of the input field in `rofi`, press `Enter` so that your search keyword appears as a list item in `rofi`. Then, click on the list item to send the request to the API.
```

