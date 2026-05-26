# Learning Notes and Commands for Basic Cryptography and Basic Forensic Analysis: OverTheWire.

## Level 11: Basic Cryptography (ROT13)
At this level, which was quite confusing, I learned that messages can be "disguised" by moving letters of the alphabet. 
In this case, it was done using the alphabet and the concept of ROT13, or a 13-position rotation.

* **Concept:** **ROT13** (13-position rotation of the alphabet A-Z).

* **Key Tool:** The `tr` (translate) command.

* **Resolution Command:**
``bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m' ```
* **Lesson:** The `tr` command is bidirectional in ROT13; The same command encrypts and decrypts, but in this case, 
it changed the letters in certain positions (for example, changing A to N). It works with both uppercase and lowercase letters.

---

## Level 12: Forensic Analysis and Decompression
This level was like peeling an "infinite onion" of compressed files, which was incredibly frustrating since there 
were .gz, .bz2, and .tar files. Each one had to be decompressed to reach the ASCII text file and decrypt the password.

### Tools used in this module.

| Command | Function |


:--- | :--- |

`xxd -r` | Converts a hexadecimal dump into a real binary file.


`file` | Identifies the actual file type regardless of its extension.


`mktemp -d` | Creates a secure temporary directory with a random name. |

`mv` | Used to add extensions (`.gz`, `.bz2`, `.tar`) so that commands work. |

### Decompression Dictionary
| File Type | Extension | Command to extract |

:--- |:--- |:--- |

**Gzip** | `.gz` | `gunzip file.gz` |

**Bzip2** | `.bz2` | `bunzip2 file.bz2` |

**Tar Archive** | `.tar` | `tar -xf file.tar` |

--

## IMPORTANT NOTES TO REMEMBER.

1. **The extension lies, the `file` command doesn't:** Never trust a filename in Linux; always use `file` to find out what it is.

2. **Recursion:** Security challenges often have hidden layers within other layers.

---
