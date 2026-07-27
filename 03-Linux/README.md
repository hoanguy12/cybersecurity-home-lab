## Relative and Absolute Paths

### Objective

Learn how to locate files and directories using relative and absolute paths.

### Concepts Learned

- Relative paths
- Absolute paths
- Current directory (`.`)
- Parent directory (`..`)
- Root directory (`/`)
- Home directory (`~`)
- How Linux interprets file paths based on the current working directory

### Hands-On Practice

- Created a practice directory called `linux-practice`
- Created a `documents` directory inside `linux-practice`
- Created a file named `linux-notes.txt` inside `documents`
- Used the `cat` command to read `linux-notes.txt`
- Accessed the same file using relative and absolute paths
- Used `cd ..` to move to the parent directory

### Challenge and Solution

I ran:
`cat documents/linux-notes.txt`
but I got the error:
`No such file or dir`
My current dir was: 
`/home/ubuntu-lab`
Because the command used a relative path, Linux looked for the file here:
`/home/ubuntu-lab/documents/linux-notes.txt`. (Shown on 2nd screenshot)
However, the file was actually located here:
`/home/ubuntu-lab/linux-practice/documents/linux-notes.txt`
I corrected the command by using the proper relative path:
`cat linux-practice/documents/linux-notes.txt`
This process is shown in the second screenshot.

### Screenshot

![](screenshots/linux-filesystem-navigation2.png)
![](screenshots/relative-vs-absolute-paths.png)

### Lessons Learned

Linux directories are organized like branches on a tree. A relative path begins from my current location, so I need to understand where I am and how the destination connects to it. An absolute path begins from the root directory `/`, so it gives the complete location and can be used no matter which directory I am currently in.
