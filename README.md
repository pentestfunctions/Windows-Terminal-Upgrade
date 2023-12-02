# Tabby with Quick Commands plugin and Kali Tool Installation

![GitHub release (latest by date)](https://img.shields.io/github/v/release/Eugeny/tabby)
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Eugeny/tabby/CI)
![GitHub](https://img.shields.io/github/license/Eugeny/tabby)
![GitHub last commit](https://img.shields.io/github/last-commit/Eugeny/tabby)

Enhance your penetration testing efficiency with Tabby and a set of essential Kali tools. This guide includes steps for installing Tabby, configuring Quick Commands plugin, and installing additional penetration testing tools in Kali.

<p align="center">
  <img src="static/quick.gif">
</p>

## Installation

### Tabby
1. Download Tabby: ![Download Tabby](https://img.shields.io/github/downloads/Eugeny/tabby/total)
   - [Latest Release](https://github.com/Eugeny/tabby/releases/latest)
2. Install Tabby.
3. Go to settings (Gear wheel in top right).
   - Click Plugins.
   - Search for "Quick Commands" and install the plugin.
   - After relaunching Tabby, go to Settings and click on Config file.
   - Paste in the config from the GitHub repository.

### Optional Configuration
Configure each new tab in Tabby:
1. Click on the settings (Gear wheel in top right).
2. Select "Profiles & Connections".
3. Choose the default connection for new tabs (WSL, SSH session, etc.).

## Kali Tools Installation
Install additional tools for Kali:
```bash
wget https://github.com/RustScan/RustScan/releases/download/2.0.1/rustscan_2.0.1_amd64.deb -O ~/Downloads/rustscan_2.0.1_amd64.deb
sudo dpkg -i ~/Downloads/rustscan_2.0.1_amd64.deb
sudo apt install gobuster
sudo apt install wordlists
sudo apt-get install dirbuster
sudo gunzip /usr/share/wordlists/rockyou.txt.tz
```

## Quick Commands Configuration
Configure Quick Commands for efficient testing:
- [Quick Commands Config](https://github.com/pentestfunctions/Windows-Terminal-Upgrade)

<details>
<summary>Sample Commands</summary>

```yaml
qc:
  cmds:
    - name: Clear the screen
      text: clear
      ...
```

</details>
