# Duplicate Remover

Duplicate Remover is a straightforward Python script designed to remove duplicate items from a text file and save the unique items to a new file.

### Installation and Usage

#### Windows

1. **Ensure Python is Installed:**
   - If Python is not already installed on your system, download it from [python.org](https://www.python.org/downloads/) and follow the installation instructions.
   - During the installation, ensure to check the box that says "Add Python to PATH".

2. **Install Git:**
   - Download the Git installer for Windows from [git-scm.com](https://git-scm.com/download/win).
   - Run the installer and follow these steps during the installation process:
     - Select "Use Git from the Windows Command Prompt" when asked about adjusting your PATH environment.
     - You can leave other options at their default settings or adjust them according to your preference.

3. **Add Git to the PATH Environment Variable (if necessary):**
   - If Git is installed but not recognized, it's likely not added to the PATH environment variable. Adding Git to the PATH allows the system to locate the Git executable from any command line interface.

   **Find Git installation path:**
   - The default installation path is usually `C:\Program Files\Git\cmd`. Verify this location exists or find where Git is installed on your machine.

   **Edit system PATH:**
   - Open the Start Menu, type `env`, and choose "Edit the system environment variables".
   - In the System Properties window, click on "Environment Variables".
   - Under "System variables", scroll to find the "Path" variable and select it, then click "Edit".
   - Click "New" and paste the path to your Git cmd folder (e.g., `C:\Program Files\Git\cmd`).
   - Click "OK" to close all dialogs and apply these changes.

   **Verify the change:**
   - Close and reopen your Command Prompt or PowerShell and type:
     ```bash
     git --version
     ```
   - You should see the version of Git installed, confirming that Git is installed and added to the PATH.

4. **Clone the Repository:**
   ```bash
   git clone https://github.com/daniyalusman/duplicate-remover/
   ```

5. **Navigate to the Directory:**
   ```bash
   cd duplicate-remover
   ```

6. **Run the Script:**
   - Double-click the `duplicate_remover.py` file to run it, or open a command prompt and execute:
     ```bash
     python duplicate_remover.py
     ```

7. **Enter the Absolute File Path:**
   - Provide the full path to the text file you want to process when prompted.

8. **Result:**
   - The script will read the file, remove duplicates, and save the unique items to `duplicate_removed.txt` in the same directory.
   - You will see a confirmation message indicating the file has been saved successfully or an error message if the file does not exist.

#### Linux

1. **Install Python:**
   - If Python is not already installed on your system, you can install it using the package manager specific to your Linux distribution. For example, on Ubuntu or Debian-based systems, you can use:
     ```bash
     sudo apt update
     sudo apt install python3
     ```

2. **Install Git:**
   - On Ubuntu or Debian-based systems, you can install Git using:
     ```bash
     sudo apt update
     sudo apt install git
     ```
   - For other distributions, use the appropriate package manager for your system.

3. **Clone the Repository:**
   ```bash
   git clone https://github.com/daniyalusman/duplicate-remover/
   ```

4. **Navigate to the Directory:**
   ```bash
   cd duplicate-remover
   ```

5. **Run the Script:**
   - Open a terminal and execute:
     ```bash
     python3 duplicate_remover.py
     ```

6. **Enter the Absolute File Path:**
   - Provide the full path to the text file you want to process when prompted.

7. **Result:**
   - The script will read the file, remove duplicates, and save the unique items to `duplicate_removed.txt` in the same directory.
   - You will see a confirmation message indicating the file has been saved successfully or an error message if the file does not exist.

## Example

Suppose you have a file `sample.txt` with the following content:

```
apple
banana
apple
orange
banana
```

Running the script on `sample.txt` will produce `duplicate_removed.txt` containing:

```
apple
banana
orange
```

## Notes

- Make sure Python is installed on your system and added to your PATH environment variable.
- This script assumes the input file is a text file where each line is treated as a separate item.
