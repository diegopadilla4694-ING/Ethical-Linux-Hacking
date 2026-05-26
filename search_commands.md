# Search Commands and Command Manual.

---

# `man` (System Manual).
Displays the complete documentation for a command, along with its options and a parameter.

* **Basic Usage:** `man <command>`
* **Press the **`q`** key to exit the manual.

### `whatis`.
Gives you a quick, one-line definition of an exact command, very effective for telling you what the selected command does.

* **Basic Usage:** `whatis <command>` (This is equivalent to using `man -f <command>`).

### `apropos`.
I use this command to search for commands I don't remember very well but have a general idea of.

* **Basic Usage:** `apropos <word>`
* **Search for an Exact Phrase:** `apropos "list directory"`

---

## 2. File Location.

whereis` This tells you the exact physical path where a program's binary (executable) and its manual are installed.
