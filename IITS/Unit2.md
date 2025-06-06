## UNIT 2: OS Installation (Linux and MS Windows), Unix Shell and Commands, vi Editor

This unit focuses on practical aspects of operating systems, specifically installation procedures for common operating systems (Linux and Windows), fundamental command-line interaction in Unix-like environments, and basic text editing using the `vi` editor.

### I. OS Installation (Linux and MS Windows)

Operating System (OS) installation is the process of setting up an operating system on a computer's hard drive or other storage device. This makes the computer usable and allows users to run applications.

#### A. Common Pre-requisites for OS Installation (General)

Before installing any OS, consider these:

* **System Requirements:** Ensure the computer meets the minimum CPU, RAM, and storage requirements for the chosen OS version.
* **Backup Data:** Crucial! All data on the target drive might be lost during installation.
* **Installation Media:** Obtain the OS installer (USB drive, DVD, or ISO file).
* **Boot Order:** Configure the computer's BIOS/UEFI settings to boot from the installation media first.
* **Internet Connection:** Often needed for updates, drivers, and software during/after installation.
* **Product Key (for Windows):** If applicable, have your Windows product key ready.
* **Partitioning Plan:** Decide how you want to divide your hard drive (e.g., single OS, dual boot, separate partitions for OS and data).

#### B. Linux Installation (General Steps)

Linux distributions (e.g., Ubuntu, Fedora, Debian) share similar installation processes. We'll use Ubuntu as a common example.

1.  **Download ISO Image:** Download the desired Linux distribution's ISO file from its official website.
2.  **Create Bootable USB/DVD:** Use tools like Rufus (for Windows) or Etcher (cross-platform) to create a bootable USB drive from the ISO.
3.  **Boot from Installation Media:** Insert the bootable USB/DVD and restart your computer. Access the BIOS/UEFI (usually by pressing F2, F10, F12, Del during startup) to change the boot order to prioritize the USB/DVD.
4.  **Live Environment/Installer:** Most Linux distros offer a "Try before you install" live environment. This lets you test the OS without installing. To install, look for an "Install" icon or option.
5.  **Language and Keyboard Layout:** Select your preferred language and keyboard layout.
6.  **Network Configuration:** Connect to a Wi-Fi network if available.
7.  **Installation Type (Partitioning):**
    * **Erase disk and install Linux:** Easiest option, dedicates the entire drive to Linux (deletes everything else).
    * **Install Linux alongside Windows (Dual Boot):** The installer resizes existing Windows partitions and creates new ones for Linux.
    * **Something else (Manual Partitioning):** For advanced users, allows full control over creating, deleting, and resizing partitions. This is necessary for specific setups or if you want to reuse existing partitions. Requires creating at least a root partition (`/`) and a swap partition. A separate home partition (`/home`) is often recommended.
8.  **Location and Time Zone:** Select your geographical location for accurate time zone settings.
9.  **User Creation:** Set up your username, computer name, and password. This will be your login credential.
10. **Installation Process:** The installer copies files, configures settings, and installs the bootloader (GRUB for Linux).
11. **Restart:** Once installation is complete, remove the installation media and restart the computer. It should now boot into Linux (or present a GRUB menu for dual-boot systems).

#### C. MS Windows Installation (General Steps, e.g., Windows 10/11)

1.  **Download Windows ISO/Create Installation Media:** Download the Windows Media Creation Tool from Microsoft's website. This tool can download the ISO and create a bootable USB drive directly.
2.  **Boot from Installation Media:** Insert the bootable USB/DVD and restart your computer. Access the BIOS/UEFI (usually by pressing F2, F10, F12, Del) to set the boot order.
3.  **Windows Setup:**
    * **Language, Time, and Keyboard:** Select your preferences.
    * **Install now:** Click to begin.
    * **Product Key:** Enter your Windows product key (or select "I don't have a product key" if you plan to activate later).
    * **Accept License Terms:** Read and accept the EULA.
    * **Installation Type:**
        * **Upgrade:** Keeps your files, settings, and apps (if upgrading an existing Windows installation).
        * **Custom: Install Windows only (advanced):** This is for a clean install.
4.  **Where do you want to install Windows? (Partitioning):**
    * If doing a clean install, you'll see a list of drives and partitions.
    * You can delete existing partitions, create new ones, or select an unallocated space. Windows will automatically create necessary system partitions (e.g., System Reserved, MSR, Recovery).
    * Select the partition where you want to install Windows (usually the largest one or the newly created primary partition).
5.  **Installation Process:** Windows copies files, installs features, drivers, and updates. This may involve several restarts.
6.  **Out-of-Box Experience (OOBE):** After the main installation, you'll go through setup steps for region, keyboard layout, Microsoft account login, privacy settings, and creating a local user account.
7.  **Desktop:** Once complete, you'll be presented with the Windows desktop.

### II. Unix Shell and Commands

The "shell" is a command-line interpreter that provides a user interface for accessing the operating system's services. In Unix-like systems (including Linux), the shell is a powerful tool for managing files, running programs, and automating tasks.

#### A. Unix Shell

* **Definition:** A program that acts as an interface between the user and the Unix/Linux kernel. It takes commands typed by the user, interprets them, and passes them to the kernel for execution. It also displays the output of the executed commands.
* **Types of Shells:** Bash (Bourne Again Shell, most common), Zsh, Fish, Ksh, Csh.
* **Shell Prompt:** The text displayed in the terminal indicating that the shell is ready to accept a command (e.g., `$`, `#`, `user@hostname:~ $`).

#### B. Basic Unix Commands

These commands are fundamental for navigating the file system, managing files, and performing basic operations.

1.  **`ls` (list):** Lists the contents of a directory.
    * `ls`: Lists files and directories in the current directory.
    * `ls -l`: Long listing format (permissions, owner, size, date).
    * `ls -a`: Lists all files, including hidden ones (starting with `.`).
    * `ls -lh`: Long listing with human-readable file sizes.

2.  **`cd` (change directory):** Changes the current working directory.
    * `cd /home/user/documents`: Go to a specific path.
    * `cd ..`: Go up one directory level.
    * `cd ~`: Go to the user's home directory.
    * `cd -`: Go to the previous directory.

3.  **`pwd` (print working directory):** Displays the full path of the current directory.

4.  **`mkdir` (make directory):** Creates a new directory.
    * `mkdir mynewdir`: Creates a directory named `mynewdir` in the current location.
    * `mkdir -p /path/to/nonexistent/dir`: Creates parent directories if they don't exist.

5.  **`rmdir` (remove directory):** Deletes an empty directory.
    * `rmdir emptyfolder`: Deletes `emptyfolder` if it's empty.

6.  **`cp` (copy):** Copies files or directories.
    * `cp file1.txt /tmp/`: Copies `file1.txt` to the `/tmp` directory.
    * `cp -r somedir /tmp/`: Recursively copies `somedir` and its contents to `/tmp`.

7.  **`mv` (move):** Moves or renames files/directories.
    * `mv oldname.txt newname.txt`: Renames `oldname.txt` to `newname.txt`.
    * `mv file.txt /backup/`: Moves `file.txt` to the `/backup` directory.

8.  **`rm` (remove):** Deletes files or directories. **Use with caution, as deleted files are often not recoverable from the command line.**
    * `rm myfile.txt`: Deletes `myfile.txt`.
    * `rm -r mydir`: Recursively deletes `mydir` and its contents (even if not empty).
    * `rm -f myfile.txt`: Force delete (no confirmation).
    * `rm -rf dangerous_dir/`: Forcefully delete a directory and its contents recursively. (Extremely dangerous if not used carefully).

9.  **`cat` (concatenate):** Displays the content of files, or concatenates them.
    * `cat mydocument.txt`: Displays the content of `mydocument.txt`.
    * `cat file1.txt file2.txt > combined.txt`: Combines `file1.txt` and `file2.txt` into `combined.txt`.

10. **`less` / `more`:** View file content page by page.
    * `less largefile.log`: Allows scrolling forward and backward. Press `q` to exit.
    * `more largefile.log`: Only allows scrolling forward. Press `q` to exit.

11. **`echo`:** Displays a line of text.
    * `echo "Hello World"`: Prints "Hello World" to the terminal.
    * `echo $PATH`: Displays the value of the PATH environment variable.

12. **`man` (manual):** Displays the manual page for a command.
    * `man ls`: Shows the help page for the `ls` command. Press `q` to exit.

13. **`grep` (global regular expression print):** Searches for patterns in files.
    * `grep "keyword" myfile.txt`: Finds lines containing "keyword" in `myfile.txt`.
    * `grep -i "keyword" myfile.txt`: Case-insensitive search.
    * `ls -l | grep "Aug"`: Pipes the output of `ls -l` to `grep` to find lines containing "Aug" (e.g., files modified in August).

14. **`chmod` (change mode):** Changes file permissions.
    * `chmod 755 script.sh`: Gives read/write/execute to owner, read/execute to group/others. (e.g., 777 for full permissions, 644 for read/write owner, read only for others).

15. **`chown` (change owner):** Changes file ownership.
    * `chown user:group myfile.txt`: Changes owner to `user` and group to `group`.

16. **`sudo` (superuser do):** Executes a command with superuser (root) privileges.
    * `sudo apt update`: Updates package lists (requires admin password).

### III. vi Editor

`vi` (visual editor) is a powerful, modal text editor commonly found on Unix-like operating systems. It's renowned for its efficiency once mastered, though it has a steep learning curve due to its modal nature.

#### A. Modal Operation

`vi` operates in different modes:

1.  **Command Mode (Normal Mode):**
    * This is the default mode when `vi` starts.
    * Used for navigation, deleting text, copying, pasting, and issuing commands (e.g., saving, quitting).
    * Typing characters in this mode performs actions, not inserts text.
2.  **Insert Mode:**
    * Entered from Command Mode by pressing keys like `i`, `a`, `o`, `I`, `A`, `O`.
    * Used for typing and editing text normally.
    * Press `Esc` to return to Command Mode.
3.  **Last Line Mode (Ex Mode):**
    * Entered from Command Mode by pressing `:` (colon).
    * Used for executing commands that affect the entire file or for configuration (e.g., saving, quitting, search and replace).
    * Press `Enter` to execute the command.

#### B. Basic `vi` Commands

**1. Starting/Opening `vi`:**
    * `vi filename`: Opens `filename` for editing. If it doesn't exist, it creates a new file.
    * `vi`: Opens an empty `vi` session.

**2. Entering Insert Mode (from Command Mode):**
    * `i`: Insert text *before* the cursor.
    * `a`: Insert text *after* the cursor.
    * `o`: Open a *new line below* the current line and enter insert mode.
    * `O`: Open a *new line above* the current line and enter insert mode.
    * `I`: Insert text at the *beginning* of the current line.
    * `A`: Insert text at the *end* of the current line.

**3. Navigating (in Command Mode):**
    * `h`: Move cursor left.
    * `l`: Move cursor right.
    * `j`: Move cursor down.
    * `k`: Move cursor up.
    * `w`: Move to the beginning of the *next* word.
    * `b`: Move to the beginning of the *previous* word.
    * `0` (zero): Move to the beginning of the line.
    * `$`: Move to the end of the line.
    * `G`: Go to the last line of the file.
    * `gg`: Go to the first line of the file.
    * `nG` or `:n`: Go to line number `n`.

**4. Deleting (in Command Mode):**
    * `x`: Delete character under cursor.
    * `dw`: Delete word from cursor to end of word.
    * `d$`: Delete from cursor to end of line.
    * `dd`: Delete the entire current line.
    * `ndd`: Delete `n` lines.

**5. Copying (Yanking) and Pasting (in Command Mode):**
    * `yy`: Yank (copy) the current line.
    * `nyy`: Yank `n` lines.
    * `p`: Paste text *after* the cursor/line.
    * `P`: Paste text *before* the cursor/line.

**6. Undo/Redo (in Command Mode):**
    * `u`: Undo the last change.
    * `Ctrl-r`: Redo the last undone change.

**7. Saving and Quitting (in Last Line Mode - press `:` first):**
    * `:w`: Save the file.
    * `:q`: Quit `vi`. (Will not quit if changes are unsaved).
    * `:wq`: Save and quit.
    * `:x`: Save and quit (similar to `:wq`).
    * `:q!`: Quit without saving (force quit).
    * `:w! filename`: Save the file with a new name (force overwrite if `filename` exists).

**8. Search (in Last Line Mode - press `:` first):**
    * `/pattern`: Search forward for `pattern`.
    * `?pattern`: Search backward for `pattern`.
    * `n`: Go to the next match (forward).
    * `N`: Go to the previous match (backward).

**9. Find and Replace (in Last Line Mode - press `:` first):**
    * `:%s/old/new/g`: Replace all occurrences of `old` with `new` throughout the entire file.
        * `%`: operate on all lines.
        * `s`: substitute.
        * `g`: global (replace all occurrences on each line, not just the first).
    * `:s/old/new/`: Replace the first occurrence of `old` with `new` on the current line.

Mastering `vi` requires practice, but its efficiency makes it a valuable skill for system administration and command-line environments.
