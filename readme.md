# Linux Fundamentals

## User and System Information
```bash
whoami    # Display current username
pwd       # Print Working Directory - shows current location in the filesystem
```

## File Operations
```bash
touch ragh.txt    # Create a new empty file named 'ragh.txt'
ls               # List files and directories in current directory
ls -la          # List files and directories in long format, including hidden files
                # This will show you detailed information, starting from the left: file permissions, number of links, owner name, owner group, file size, timestamp of last modification, and file/directory name.
```

## Directory Operations
```bash
mkdir ragh    # Create a new directory named 'ragh'
cd ragh/      # Change directory to 'ragh'

cd .     # . (current directory). This is the directory you are currently in.

cd ..    # .. (parent directory). Takes you to the directory above your current.

cd ~     # ~ (home directory). This directory defaults to your “home directory”. 

cd -     # - (previous directory). This will take you to the previous directory you were just at.

```
