## Relative and Absolute Paths

### Objective

Learn how to navigate directories

### Concepts Learned

- Relative Paths
- Absolute paths
- Directory Logic
- Commands

### Hands-On Practice

- Created practice dir called linux-practice containing documents containing linux-notes.txt
- Used command "cat" to read linux-notes.txt

### Challenge and Solution

I tried cat documents/linux-notes.txt, but I got the error "No such file or dir". This command looked for it at current dir: /home/ubuntu-lab, but it was actually a sub dir there: linux-practice/documents/linux-notes.txt. (Shown on 2nd screenshot)

### Screenshot

![](screenshots/linux-filesystem-navigation2.png)
![](screenshots/relative-vs-absolute-paths.png)

### Lessons Learned

The organization of dirs work like a tree branch. You must know where you are on the branch and you cannot jump from one branch to another without following the path from where it connects from and to.
