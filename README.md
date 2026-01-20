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
<img width="1470" height="956" alt="EnsureAPT" src="https://github.com/user-attachments/assets/bc03f1a8-6df3-4a16-80ce-e55d2d1ebd8d" />


---

### 2. Install the Suricata Application

Install Suricata, an open-source network threat detection engine.

```bash
sudo apt install suricata
```
<img width="1470" height="956" alt="InSuricata" src="https://github.com/user-attachments/assets/f9b9d8cc-b69d-43f7-a3b4-d33d6cdcd24a" />

* Enter your password when prompted
Confirm the installation by typing `Y` and pressing Enter

---

### 3. Verify Suricata Installation

Confirm that Suricata is installed correctly.

```bash
suricata
```

If installed successfully, Suricata’s usage or help output will appear.

<img width="1470" height="956" alt="InSuricata" src="https://github.com/user-attachments/assets/baf2351d-de30-4e2a-8d47-fd01517c843d" />


---

### 4. Uninstall the Suricata Application

Remove Suricata from the system.

```bash
sudo apt remove suricata
```

* Confirm the removal when prompted
<img width="1470" height="956" alt="Removesuri" src="https://github.com/user-attachments/assets/f07bd101-bf92-4d97-a8e8-2a5d98c17a54" />

---

### 5. Verify Suricata Uninstallation

Check that Suricata has been removed.

```bash
suricata

```

You should receive a message indicating that the command is not found or no such file exists.
<img width="1470" height="956" alt="Suricata" src="https://github.com/user-attachments/assets/e5319482-3254-416c-a3a7-0761f1040c6f" />

---

### 6. Install the TCPdump Application

Install TCPdump, a command-line packet analyzer.

```bash
sudo apt install tcpdump
```
<img width="664" height="428" alt="Installtcpdump" src="https://github.com/user-attachments/assets/bb1f7482-55f9-4631-8188-aaca59f0f8e4" />


---

### 7. List Installed Applications

Display a list of all installed packages on the system.

```bash
apt list --installed
```

<img width="659" height="430" alt="APTlist" src="https://github.com/user-attachments/assets/ec80413f-979f-4164-b1c6-f0ea11ab1d29" />



This command helps verify installed software and track system packages.

---

### 8. Reinstall the Suricata Application

Reinstall Suricata on the system.

```bash
sudo apt install suricata
```


<img width="1470" height="956" alt="Rein" src="https://github.com/user-attachments/assets/c03d7402-4a16-4a91-903a-e95be26e28b3" />



---

### 9. Verify Installed Applications Again

Confirm that Suricata appears in the installed package list.

```bash
apt list --installed
```

<img width="726" height="413" alt="Done" src="https://github.com/user-attachments/assets/ba12368f-8729-426e-867f-ec8785765405" />


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
