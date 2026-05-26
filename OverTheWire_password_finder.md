# OverTheWire Password Cracking Commands

## Tools Learned
At these levels, I mastered the use of pipes (`|`) and parameters (`-`) to process information.

### Main Command Table
| Commands Used | Function | Use at each level completed and documented |

:--- |:--- |:--- |

`cat` | Open files | A very common command that I have mastered, which only displays the contents of the file `data.txt`. |

`grep` | Filter text | Search for specific patterns requested by the user, such as `==`. |

`sort` | Sort | Groups repeated lines alphabetically. |

`uniq` | Filter duplicates | This command searches for the only line that is not repeated with `-u`. 
(Note: `uniq` and `-u` are good commands for searching and extracting lines that are not repeated) |

`strings` | Extract text that is understandable in human language | Extract all readable words from the 
binary files I am searching for (Level 9). |

`base64` | Decode | Translate Base64 code into text or a language I can understand in order to 
decrypt the password `-d` (Level 10). |

---

## Key Levels (Important to master).

### Level 8: The Unique Filter
**Challenge:** This challenge involved finding a single line that was not the same as the others within the .txt file provided by the website.

**Final Command:**
``` cat data.txt | sort | uniq -u
