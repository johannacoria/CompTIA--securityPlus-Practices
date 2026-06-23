Coursera: Linux Tools of the Trade – Software Installation in Linux

Lab: Installing and Managing Software on a Linux System

Objective

Learn how to manage the software lifecycle in a Debian/Ubuntu-based Linux distribution using the Advanced Package Tool (APT). This includes verifying package manager availability, installing security tools, removing packages, and reinstalling software as part of basic system administration workflows.

Tools Used

* APT (Advanced Package Tool): Package management system used in Debian-based Linux distributions for installing, updating, and removing software while automatically resolving dependencies.
* Suricata: Open-source network intrusion detection and prevention system (IDS/IPS).
* tcpdump: Command-line packet analyzer used for network traffic inspection.

Tasks Completed

1. Verify APT Installation

Before performing any package management operations, the availability of APT was verified in the system:

apt --version

This confirms that the package management system is installed and operational.

2. Install Suricata using APT

Suricata was installed from the official repositories using APT:

sudo apt-get update
sudo apt-get install suricata

* apt-get update ensures the local package index is synchronized with remote repositories.
* apt-get install downloads and installs the specified package along with its dependencies.

3. Remove Suricata using APT

Suricata was uninstalled from the system:

sudo apt-get remove suricata

This command removes the package while preserving configuration files by default.

4. Install tcpdump using APT

tcpdump was installed to analyze network traffic at the packet level:

sudo apt-get install tcpdump
_

5. Reinstall Suricata using APT

Suricata was reinstalled to reinforce understanding of package lifecycle management:

sudo apt-get install suricata


Key Takeaways

* Learned how to verify system package manager availability.
* Understood the software lifecycle in Linux systems (install, remove, reinstall).
* Practiced using APT to manage security and networking tools.
* Gained familiarity with system-level tools used in cybersecurity environments.

Conclusion

This lab provided foundational experience in Linux system administration using APT. Managing tools such as Suricata and tcpdump helped reinforce practical knowledge of installing and maintaining security-focused software in a Debian-based environment.
