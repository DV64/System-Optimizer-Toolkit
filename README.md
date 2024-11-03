# README - System Optimizer Toolkit 1.5

## Introduction
The System Optimizer Toolkit is a comprehensive utility designed to improve the performance of Windows operating systems. It provides a user-friendly interface for performing various system checks, optimizations, and maintenance tasks. This toolkit is particularly useful for users looking to enhance their system's efficiency, troubleshoot issues, and gather detailed information about their hardware and software configurations.

## Requirements
- **Operating System**: Windows (Windows 7 or newer is recommended).
- **Administrator Privileges**: Some functionalities require the script to be run with administrator rights to access system-level information and make changes.

## How to Use
1. **Download the Script**: Save the `SystemOptimizer.bat` file to a directory of your choice on your computer.
2. **Run as Administrator**: 
   - Right-click on the `SystemOptimizer.bat` file.
   - Select "Run as administrator" to ensure the script has the necessary permissions to execute all features.
3. **Follow On-Screen Instructions**: The script will present a menu with various options. You can enter the number corresponding to the desired action.

## Features Overview
The toolkit is divided into several categories, each containing specific tools and functionalities:

### 1. Information Tools
These tools provide detailed insights into your system's hardware and software configurations.

- **View System Information**: 
  - Displays general system information such as OS version, processor details, memory statistics, and disk drives.
  - Utilizes the `systeminfo` command and `wmic` for detailed hardware information.

- **Internet Test**: 
  - Pings a reliable external server (e.g., Google) to check internet connectivity.
  - Logs the result to indicate whether the connection is stable or if there are issues.

- **TPM 2.0 Check**: 
  - Checks if the Trusted Platform Module (TPM) version 2.0 is supported and enabled on the system.
  - Important for security features in Windows 11 and BitLocker encryption.

- **Check Windows 11 Compatibility**: 
  - Evaluates the system against the requirements for Windows 11, including processor compatibility, TPM status, and memory availability.

- **Battery Health Check**: 
  - Generates a battery report using the `powercfg` command, providing insights into battery health and performance.
  - The report is saved as an HTML file in the user's directory.

- **Memory (RAM) Test**: 
  - Initiates the Windows Memory Diagnostic Tool to check for memory issues.
  - Prompts the user to restart the computer to perform the test.

- **Disk Health Check**: 
  - Uses PowerShell to retrieve S.M.A.R.T. data from physical disks, assessing their health status.

- **Graphics Card Info**: 
  - Displays information about the installed graphics card, including its name, driver version, and memory.

- **CPU Stress Test**: 
  - Provides guidance on using third-party software (e.g., Prime95) for stress testing the CPU.

- **Operating System Version**: 
  - Displays the current OS version, build number, and edition.

- **Update Check**: 
  - Opens the Windows Update settings to allow the user to check for and install updates.

- **System Uptime**: 
  - Shows how long the system has been running since the last boot.

- **Firewall Status**: 
  - Provides detailed status information about the Windows Firewall for all profiles (Domain, Private, Public).

- **User  Account Control (UAC) Status**: 
  - Checks and displays the status of User Account Control settings.

### 2. Optimization Tools
These tools focus on improving system performance and cleaning up unnecessary files.

- **Delete Temp Files**: 
  - Cleans up temporary files from both the user and Windows temp directories to free up disk space.
  - Logs the actions taken during the cleanup process.

- **Scan for Unwanted Programs**: 
  - Generates a list of installed programs and checks for potentially unwanted programs (PUPs) based on common keywords.
  - Provides a report for user review.

- **Optimize System Performance**: 
  - Disables unnecessary startup programs to improve boot time.
  - Sets the power plan to high performance for better responsiveness.
  - Cleans temporary files and disables unnecessary services.
  - Checks for outdated drivers and prompts the user for updates.

### 3. Maintenance Tools
These tools assist in troubleshooting and maintaining system integrity.

- **Internet Connection Issues**: 
  - Provides troubleshooting steps to diagnose and fix internet connectivity problems.
  - Tests local network connectivity and external DNS resolution.

- **System File Corruption**: 
  - Runs the System File Checker (SFC) to scan for and repair corrupted system files.
  - Optionally runs the DIS M tool to fix corrupted system images.

- **Application Issues**: 
  - Opens the Event Viewer to display application-specific logs for troubleshooting purposes.

### 4. Developer Information
- **Name**: Dark Virus
- **Email**: N/A
- **GitHub Profile**: github.com/DV64

## Logging
All activities, errors, and results are logged in the `logfile.log` located in the same directory as the program. You can review this file for details on the operations performed.

## Notes
- **Run as Administrator**: Ensure to run the script as an administrator for all necessary permissions.
- **System Restart**: You may need to restart your system after using some tools.

---

**Disclaimer**: This program is a utility tool, and the developer is not responsible for any issues that may arise from its use.
