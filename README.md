# MyUnattend

Personal `autounattend.xml` files for creating minimal, debloated, and customized Windows 11 Pro installations.

---

## Configurations

### 1. `Personal-Desktop.xml`
Optimized for a daily driver physical workstation. It automates the OS setup but leaves user account creation to you.

* **Interactive User Setup**: Prompts you to create a user account.
* **Aggressive Debloating**: Removes 40+ built-in apps and features like Copilot, Teams, and OneDrive.
* **Security Tweaks**: Disables Microsoft Defender and hardens C: drive permissions.
* **UI Enhancements**: Restores the classic context menu, sets the taskbar to the left, and shows all file extensions.
* **Locale**: `en-US` UI with `sv-SE` (Swedish) locale and keyboard.

### 2. `Virtual-Machine.xml`
Designed for quickly creating disposable virtual machines for testing or development. It prioritizes performance and convenience.

* **Fully Automated User**: Creates a passwordless `Admin` user and logs in automatically.
* **Optimized for Performance**: All visual effects are disabled, and System Restore is removed.
* **VM-Specific Features**: Enables Remote Desktop (RDP) and auto-installs VMware Tools if the ISO is attached.
* **Reduced Security**: Disables Defender, SmartScreen, and Smart App Control for lab environments.
* **Desktop Icons**: Adds "This PC" and "Control Panel" to the desktop.

---

## How to Use

1.  Create a bootable Windows 11 USB drive using a tool like Rufus.
2.  Download a configuration file from this repository.
3.  Rename it to **`autounattend.xml`**.
4.  Place the file on the root of the bootable USB drive.
5.  Boot from the USB drive to start the automated installation.

---

## Disclaimer

These configurations make significant changes to the OS, including the **complete removal of Microsoft Defender**. They are provided as-is. Use at your own risk and understand the changes being made to your system.
