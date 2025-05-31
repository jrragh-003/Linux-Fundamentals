# Linux Fundamentals

## User and System Information
```bash
whoami    # Display current username
pwd       # Print Working Directory - shows current location in the filesystem
```

## File Operations
```bash
touch ragh.txt    # Create a new empty file named 'ragh.txt'
ls                # List files and directories in current directory
ls -la            # List files and directories in long format, including hidden files
                  # This will show you detailed information, starting from the left: file permissions, number of links, owner name, owner group, file size, timestamp of last modification, and file/directory name.
```

## Directory Operations
```bash
mkdir ragh    # Create a new directory named 'ragh'
mkdir -p ragh/books/favourites

cd ragh/      # Change directory to 'ragh'

cd .     # . (current directory). This is the directory you are currently in.

cd ..    # .. (parent directory). Takes you to the directory above your current.

cd ~     # ~ (home directory). This directory defaults to your “home directory”. 

cd -     # - (previous directory). This will take you to the previous directory you were just at.

```

## Copy Operations
```bash
cp *.jpg /home/ragh/Pictures
# * the wildcard of wildcards, it's used to represent all single characters or any string.
# ? used to represent one character
# [] used to represent any character within the brackets

cp -r Pumpkin/ /home/ragh/Documents    #This will recursively copy the files and directories within a directory
cp -i mycoolfile /home/ragh /Pictures  #Use the -i flag (interactive) to prompt you before overwriting a file.
```

## Move Operations
```bash
mv oldfile newfile              # Rename files
mv file2 /home/ragh/Documents   # Move a file to a different directory
mv file_1 file_2 /somedirectory # Move more than one file

mv directory1 directory2        # Rename Directories
mv -i directory1 directory2     # Use the -i flag to prompt you before overwriting anything.

#Let’s say you did want to mv a file to overwrite the previous one. You can also make a backup of that file and it will just rename the old version with a ~.
mv -b directory1 directory2
```

## Remove Operations
```bash
rm file1             # Used to delete files and directories.
rm -f file1          # Force remove file
rm -i file           # Will give you a prompt on whether you want to actually remove the files or directories.
rm -r directory      # Recursively remove all files and subdirectories it may have
rmdir directory      # Remove a directory
```
## Finding files/directories
```bash
find /home -name stars.jpg       # Specify the directory where the file needs to be searched
find /home -type d -name MyFolder # Type of the file to find. (d) for directory.
```

