# sboports
**A Simple Shell-based Ports-like Manager for SlackBuilds.org Scripts**

`sboports` is a small, command-line utility written in **Shell Bash** to simplify the process of working with the **SlackBuilds.org ("SBo")** repository. It functions as a lightweight, **ports-like** system, allowing users to clone, update, and manage the SBo script tree.

Like other Slackware-centric tools, `sboports` deliberately **does not handle dependency checking or resolution** by default. It assumes the user is aware of the package's requirements as listed in the `.info` file.

The core design principle is to make it easy to perform the manual steps of SBo package management, specifically:
1.  Keeping the SBo repository synchronized.
2.  Automating the **Download -> Checksum -> Build -> Install** cycle for a package located in the correct directory.

**Usage**

All commands are executed directly from the command line. Most package-specific commands (`fetch`, `checksum`, `install`, `uninstall`, `clean`) **must be executed from within the package's directory** (e.g., `/usr/ports/multimedia/vlc`).

Typing `sboports help` will display the full command-line options and usage information.
