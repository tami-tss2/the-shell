# The Bash Shell

Notes from the tutorial videos at Drupalize.me.

These tutorials cover the basics of a \*nix command line. The \*nix shell include Linux, Mac OS, and Cygwin or Git Bash on Windows.

---

## [1] Moving Around the Command Line

This section covers basic understanding of the prompt, and how to navigate around in the shell.

### Understanding the Prompt

The prompt shows the user, the shell name, and the current directory.

My Git Bash shell prompt is `tss2@NBILL-TSS2 MINGW64 ~`.

This indicates three pieces of information:

- `tss2@NBILL-TSS2` is the name of the computer
- `MINGW64` is the name of the shell
  - Ubuntu prompt is `tss2@NBILL-TSS@:~`
  - Powershell prompt is `PS C:\Users\tss2>`
  - Command Line prompt is `C:\Users\tss2>`
- `~` is the current directory.
  - The `~` symbol indicates the home directory on the system.

### Print Working Directory (pwd)

The `pwd` command will print the path to the current directory.

```sh
pwd
>> /c/Users/tss2
```

The prompt indicates a current directory of `~`. The `pwd` command shows a current directory located at `/c/Users/tss2`. Therefore, on this computer, in this shell, `~` is equivalent to `/c/Users/tss2`.

### List Stuff (ls)

The `ls` command lists all of the files and folders in the current directory.

The GUI (File Explorer) typically hides hidden files from view, but the command line does not, so you will see hidden files listed here as well.
Hidden file names start with a `.`.

Example of the `ls` command.

```sh
tss2@NBILL-TSS2 MINGW64 /C/Users/tss2/Desktop/TheShell

$ ls
dir1/  dir1_copy/  exie.exe*  stats/  The-Bash-Shell.md

$ ls -a ./  ../  dir1/  dir1_copy/  exie.exe*  stats/  The-Bash-Shell.md

$ ls -l
total 13
drwxr-xr-x 1 tss2 1049089    0 Dec 30 16:04 dir1/
drwxr-xr-x 1 tss2 1049089    0 Dec 30 16:28 dir1_copy/
-rwxr-xr-x 1 tss2 1049089   18 Dec 30 17:21 exie.exe*
drwxr-xr-x 1 tss2 1049089    0 Dec 30 16:08 stats/
-rw-r--r-- 1 tss2 1049089 4193 Dec 30 18:10 The-Bash-Shell.md

$ ls -al
total 25
drwxr-xr-x 1 tss2 1049089    0 Dec 30 17:21 ./
drwxr-xr-x 1 tss2 1049089    0 Dec 30 15:45 ../
drwxr-xr-x 1 tss2 1049089    0 Dec 30 16:04 dir1/
drwxr-xr-x 1 tss2 1049089    0 Dec 30 16:28 dir1_copy/
-rwxr-xr-x 1 tss2 1049089   18 Dec 30 17:21 exie.exe*
drwxr-xr-x 1 tss2 1049089    0 Dec 30 16:08 stats/
-rw-r--r-- 1 tss2 1049089 4478 Dec 30 18:11 The-Bash-Shell.md
```

See also: `ls --help` in the shell.

<!-- Links to the resournces -->

<!-- 1. Moving Around the Command Line -->

[1]: https://drupalize.me/videos/moving-around-command-line?p=1149
