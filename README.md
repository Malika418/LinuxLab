**Loom Walkthrough Video:**
[https://loom.com/share/1f54a633070042b8832558c4c0c826a0](https://loom.com/share/1f54a633070042b8832558c4c0c826a0)
# LinuxLab
# Installing and Uninstalling Applications Using APT in Linux

## Objective

This activity demonstrates how to install, verify, uninstall, and manage applications using the **APT (Advanced Package Tool)** package manager in a Linux distribution. APT is commonly used in Debian-based systems such as Ubuntu to manage software packages securely and efficiently.

---

## Prerequisites

* Linux system (Ubuntu/Debian-based)
* Terminal access
* Sudo (administrator) privileges
* Internet connectivity

---

## Step-by-Step Procedure

### 1. Ensure APT Is Installed

Verify that APT is available on the system.

```bash
apt
```

If APT is installed, a list of available commands and usage information will be displayed.

---

### 2. Install the Suricata Application

Install Suricata, an open-source network threat detection engine.

```bash
sudo apt install suricata
```

* Enter your password when prompted
* Confirm the installation by typing `Y` and pressing Enter

---

### 3. Verify Suricata Installation

Confirm that Suricata is installed correctly.

```bash
suricata
```

If installed successfully, Suricata’s usage or help output will appear.

---

### 4. Uninstall the Suricata Application

Remove Suricata from the system.

```bash
sudo apt remove suricata
```

* Confirm the removal when prompted

---

### 5. Verify Suricata Uninstallation

Check that Suricata has been removed.

```bash
suricata
```

You should receive a message indicating that the command is not found or no such file exists.

---

### 6. Install the TCPdump Application

Install TCPdump, a command-line packet analyzer.

```bash
sudo apt install tcpdump
```

---

### 7. List Installed Applications

Display a list of all installed packages on the system.

```bash
apt list --installed
```

This command helps verify installed software and track system packages.

---

### 8. Reinstall the Suricata Application

Reinstall Suricata on the system.

```bash
sudo apt install suricata
```

---

### 9. Verify Installed Applications Again

Confirm that Suricata appears in the installed package list.

```bash
apt list --installed
```

---

## Cautionary Notes

* Always use `sudo` when installing or removing packages to ensure proper permissions.
* Verify package names carefully before uninstalling to avoid removing critical system software.

---

## Tips for Efficiency

* Use **tab completion** to speed up command entry.
* Regularly update package lists using:

  ```bash
  sudo apt update
  ```
* Maintain documentation of installed tools for troubleshooting and audits.


---

## Skills Demonstrated

* Linux package management
* Software installation and removal
* Command-line proficiency
* Security tooling familiarity (Suricata, TCPdump)

---

*Documented as part of hands-on Linux and cybersecurity lab practice.*
