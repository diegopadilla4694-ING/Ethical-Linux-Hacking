#My Progress in HTB Academy - Linux Fundamentals

This repository contains my notes and solutions to the Hack The Box challenges.

##Section Notes: File Navigation

### Key Concepts
* **Hidden Files:** Listed with `ls -a`. An example is `.bash_history`, which stores the user's command history.

* **Inodes (Index Numbers):** A unique identifier for a file in the file system. Viewed with `ls -i` or `stat`.

### Challenges Completed
- Identify the user's Bash history.

- Find the index number of the `/etc/sudoers` file.

### Useful Commands
| Command | Description |

| :--- | :--- |

`ssh htb-student@IP` | Secure remote connection |

| `ls -i /etc/sudoers` | View the inode number |

`stat /etc/sudoers` | Detailed file information |

--- Note: Viewing the inode number was very complicated.

