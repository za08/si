# SI - System Information Report Script

This repository contains a Bash script designed to generate a comprehensive system information report on a Linux machine. The report includes details about system hardware, software, and current operational status, all saved to an output file.

## Script Overview

The script generates a report with the following sections:

1. **System Information**: General system information provided by `hostnamectl`.
2. **CPU Information**: Detailed information about the CPU using `lscpu`.
3. **Memory Information**: Current memory usage displayed by `free -h`.
4. **Disk Usage**: Disk space usage across all mounted filesystems via `df -h`.
5. **Network Interfaces**: Information about network interfaces using `ip addr`.
6. **Installed Packages**: A list of installed packages (for Debian-based systems) using `dpkg --get-selections`.
7. **System Logs**: The last 50 lines of the system log from `/var/log/syslog`.
8. **Running Processes**: A snapshot of all running processes using `ps aux`.
9. **Loaded Kernel Modules**: A list of currently loaded kernel modules via `lsmod`.
10. **System Uptime**: How long the system has been running using `uptime`.

## Output

The report is saved to a file named `si.txt` in the same directory where the script is executed. The report includes section headers for clarity.

## How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   ```
2. Make the script executable:
   ```bash
   chmod +x system_info.sh
   ```
3. Run the script:
   ```bash
   ./system_info.sh
   ```
4. After execution, the report will be saved to `si.txt` in the current directory.

## Compatibility

- The script is designed to run on Linux systems.
- The `Installed Packages` section only works on Debian-based systems (e.g., Ubuntu). If the system is not Debian-based, this section will be skipped.

## Contributing

Feel free to fork this repository and submit pull requests to improve the script or add new features.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

You can customize the repository name, username, or any other details as needed.
