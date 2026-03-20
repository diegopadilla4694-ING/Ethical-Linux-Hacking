# File Management in Linux (HTB Academy)
## Module: Creating, Moving, and Copying

In this section, I learned how to manipulate the directory and file structure from the 
Linux terminal with the help of the Hack the Box course.

### Creating Files and Directories

** Use `tree` to visualize the folder structure graphically, and use the dot to show the 
complete structure of the current directory.

### Moving and Renaming (`mv`)
The `mv` command is versatile: it can be used to change both the name and the location of a file.

* **Rename:**

`mv info.txt information.txt`

* **Move to a directory:**

`mv information.txt Storage/`
* **Move multiple files at once:**

`mv file1.txt file2.txt Destination/`

### Copy Files (`cp`)
Creates a duplicate of the file in the specified path without deleting the original, which is very useful if you want to have a file in a different directory than the one you are currently using.

* **Syntax:** `cp <source> <destination>`
* **Example:** `cp Storage/readme.txt Storage/local/`

### Final Structure Summary
After practicing with the `tree` command, it looks like this:
```bash

` ... └── Storage 
├── information.txt 
├── local 
│ ├── readme.txt <-- Copied here 
│ └── user 
│ ├── documents 
│ └── userinfo.txt 
└── readme.txt <-- Original here

