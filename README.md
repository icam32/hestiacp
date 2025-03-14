![Hestia screenshot](https://hestiacp.com/img/screen_HestiaServer-dark.png)

[Hestia Control Panel](https://www.hestiacp.com/)
==================================================
**Latest stable release:** Version 1.6.4 | [View Changelog](https://github.com/hestiacp/hestiacp/blob/release/CHANGELOG.md) | [![Build Status](https://drone.hestiacp.com/api/badges/hestiacp/hestiacp/status.svg?ref=refs/heads/main)](https://drone.hestiacp.com/hestiacp/hestiacp) <br>

**Web:** [www.hestiacp.com](https://www.hestiacp.com/)<br>
**Documentation:** [docs.hestiacp.com](https://docs.hestiacp.com/)<br>
**Forums:** [forum.hestiacp.com](https://forum.hestiacp.com/)<br>
**Discord:** [Join the discussion](https://discord.gg/nXRUZch)<br />
<br>
[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ST87LQH2CHGLA)<br /><br />
Bitcoin : bc1q48jt5wg5jaj8g9zy7c3j03cv57j2m2u5anlutu<br>
Ethereum : 0xfF3Dd2c889bd0Ff73d8085B84A314FC7c88e5D51<br>
Binance: bnb1l4ywvw5ejfmsgjdcx8jn5lxj7zsun8ktfu7rh8<br>
Smart Chain: 0xfF3Dd2c889bd0Ff73d8085B84A314FC7c88e5D51<br>

**Welcome!**
---------------------------- 
Hestia Control Panel is designed to provide administrators an easy to use web and command line interface, enabling them to quickly deploy and manage web domains, mail accounts, DNS zones, and databases from one central dashboard without the hassle of manually deploying and configuring individual components or services. 

Features and Services
----------------------------
* Apache2 and NGINX with PHP-FPM
* Multiple PHP versions (5.6 - 8.1, 8.0 as default)
* DNS Server (Bind) with clustering capabilities
* POP/IMAP/SMTP mail services with Anti-Virus, Anti-Spam, and Webmail (ClamAV, SpamAssassin, Sieve, Roundcube)
* MariaDB and/or PostgreSQL databases
* Let's Encrypt SSL support with wildcard certificates
* Firewall with brute-force attack detection and IP lists (iptables, fail2ban, and ipset).

Supported platforms and operating systems
========================================================

* **NOTE:** Hestia Control Panel does not support 32 bit operating systems!

* **Debian:** 11 or 10
* **Ubuntu:** 22.04LTS, 20.04 LTS or 18.04 LTS

* **NOTE:** Hestia Control Panel in combination with OpenVZ 7 or lower might have issue Bind9 server not starting or issues with Firewall. If you use a Virtual Private Server we strongly advice you to use something based on KVM or LXC!

Installing Hestia Control Panel
============================

* **NOTE:** Hestia Control Panel must be installed on top of a fresh operating system installation to ensure proper functionality.

While we have taken every effort to make the installation process and the control panel interface as friendly as possible (even for new users), it is assumed that you will have some prior knowledge and understanding in the basics how to set up a Linux server before continuing.

## Step 1: Log in
To start the installation, you will need to be logged in as **root** or a user with super-user privileges. You can perform the installation either directly from the command line console or remotely via SSH:
```bash
ssh root@your.server
```
## Step 2: Download
Download the installation script for the latest release:
```bash
wget https://raw.githubusercontent.com/hestiacp/hestiacp/release/install/hst-install.sh
```
If the download fails due to an SSL validation error, please be sure you've installed the ca-certificate package on your system - you can do this with the following command:
```bash
apt-get update && apt-get install ca-certificates
```

## Step 3: Run
To begin the installation process, simply run the script and follow the on-screen prompts:
```bash
bash hst-install.sh
```
You will receive a welcome email at the address specified during installation (if applicable) and on-screen instructions after the installation is completed to log in and access your server.

## Custom installation:
You may specify a number of various flags during installation to only install the features in which you need. To view a list of available options, run:
```bash
bash hst-install.sh -h
```
Alternatively, @gabizz has made available a command-line script generator at https://gabizz.github.io/hestiacp-scriptline-generator/ which allows you to easily generate the installation command via GUI.

How to upgrade an existing installation
============================
Automatic Updates are enabled by default on new installations of Hestia Control Panel and can be managed from **Server Settings > Updates**. To manually check for and install available updates, use the apt package manager:
```bash
apt-get update
apt-get upgrade
```

Issues & Support Requests
=============================
* If you encounter a general problem while using Hestia Control Panel and need help, please [visit our forum](https://forum.hestiacp.com/) to search for potential solutions or post a new thread where community members can assist.
* Bugs and other reproducible issues should be filed via GitHub by [creating a new issue report](https://github.com/hestiacp/hestiacp/issues) so that our developers can investigate further. Please note that requests for support will be redirected to our forum.

**IMPORTANT: We _cannot_ provide support for requests that do not describe the troubleshooting steps that have already been performed, or for third-party applications not related to Hestia Control Panel (such as WordPress). Please make sure that you include as much information as possible in your forum posts or issue reports!**

Contributions
=============================
If you would like to contribute to the project, please [read our Contribution Guidelines](https://github.com/hestiacp/hestiacp/blob/release/CONTRIBUTING.md) for a brief overview of our development process and standards.

Copyright
=============================
"Hestia Control Panel", "HestiaCP", and the Hestia logo are original copyright of hestiacp.com and the following restrictions apply:

**You are allowed to:**
- use the names "Hestia Control Panel", "HestiaCP", or the Hestia logo in any context directly related to the application or the project. This includes the application itself, local communities and news or blog posts.

**You are not allowed to:**
- sell or redistribute the application under the name "Hestia Control Panel", "HestiaCP", or similar derivatives, including the use of the Hestia logo in any brand or marketing materials related to revenue generating activities,
- use the names "Hestia Control Panel", "HestiaCP", or the Hestia logo in any context that is not related to the project,
- alter the name "Hestia Control Panel", "HestiaCP", or the Hestia logo in any way.

License
=============================
Hestia Control Panel is licensed under [GPL v3](https://github.com/hestiacp/hestiacp/blob/release/LICENSE) license, and is based on the [VestaCP](https://www.vestacp.com/) project.<br>
