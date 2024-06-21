### Linux Terminal Commands

# Launching WSL from Git Bash:
	- ```winpty wsl```

# Quitting WSL from Ubuntu Terminal in Git Bash:
	- ```cd ..``` cd until at root directory
	- ```exit```

# File and Directory Commands:
	- ```ls``` : list directory contents
	- ```cd``` : change directory
	- ```pwd``` : print working directory
	- ```mkdir``` : create a new directory
	- ```rm``` : remove files or directories
		- ```rm -i <file>``` prompts for confirmation before deletion
		- ```rm -f <file>``` force removal without prompting
		- ```rm -r <directory>``` remove directories and their contents
		- ```rm -v <file>``` explains what is being done
		- ```rm -d <directory>``` remove empty directories
	- ```cp``` : copy files or directories
		- ```cp <original> <copy>``` copies file to same directory with a new name
		- ```cp <file> /home/user/documents/``` copies file to a different directory
		- ```cp <file> <file> <file> /home/user/documents/``` copies multiple files to a different directory
		- ```cp -r Projects/ /home/user/backup/``` copies directory and its contents
		- ```cp -p <original> <copy>``` copies with preservation of file attributes
		- ```cp -i <file> /home/user/documents/``` copies with confirmation prompt
		- ```cp -v <file> /home/user/documents/``` shows whats being done/copied
	- ```mv``` : move or rename files or directories
		- ```mv <old_file> <new_file>``` renames a file
		- ```mv <file> /home/user/documents/``` moves a file to a different directory
		- ```mv <file> <file> <file> /home/user/backup/``` moves multiple files to a different directory
		- ```mv <old_directory> <new_directory>``` renames a directory
		- ```mv <directory> /home/user/folder``` moves a directory and its contents
		- ```mv -b <old_file> <new_file>``` move and backup existing file
		- ```mv -u <new_file> /home/user/documents/``` moves a file only if its source file is newer
	- ```touch``` : create an empty file or update file timestamps
	- ```chmod``` : change file permissions
	- ```chown``` : change file ownership
	- ```ln``` : create links between files

# File Viewing and Editing Commands:
	- ```cat``` : display file contents
	- ```less``` : view file contents page by page
	- ```head``` : display the beginnning of a file
	- ```tail``` : display the end of a file
	- ```nano``` : text editor (for wimps)
	- ```vim``` : text editor (for people who got that dawg in them)

# File Searching and Pattern Matching Commands:
	- ```grep``` : search for patterns in files
	- ```find``` : search for files and directories
	- ```locate``` : find files by name

# System Information:
	- ```uname``` : print system information
	- ```whoami``` : print current user
	- ```id``` : print user and group information
	- ```df``` : report file system disk space
	- ```du``` : estimate file space usage
	- ```free``` : display amount of free and used memory

# Process Management:
	- ```ps``` : report process status
	- ```top``` : display and update sorted information about processes
	- ```kill``` : terminate processes
	- ```pkill``` : signal processes based on name and other attributes
	- ```bg``` : put jobs in background
	- ```fg``` : bring jobs to foreground
	- ```jobs``` : list active jobs

# System Controls:
	- ```sudo``` : execute a command as superuser
		- ```sudo apt-get install <package>``` installs software like a python interpreter
		- ```sudo vim /etc/ssh/sshd_config``` edit a system config file
		- ```sudo systemct1 restart apache2``` restart a system service
		- ```sudo chown <user>:<group> <file>``` change ownership of a file or directory
		- ```sudo apt update && sudo apt upgrade``` update the system
		- ```sudo mount /dev/sdb1 /mnt/usb``` mount a filesystem
		- ```sudo visudo``` view or edit the sudoers file
		- ```sudo adduser <username>``` add a new user to the system
		- ```sudo passwd <username>``` change a user's password
		- ```sudo cat /var/log/auth.log``` view the contents of a restricted file
		- ```sudo -i``` run a shell with root privileges
		- ```sudo vim /etc/hosts``` edit the hosts' files
		- ```sudo apt-get clean``` clean the package cache
		- ```sudo apt-get purge <package>``` remove a package and its config files
		- ```sudo reboot``` reboot the system
	- ```shutdown``` : shutdown or restart the system
	- ```reboot``` : reboot the system

# Networking Commands:
	- ```ifconfig``` : configure network interface parameters
	- ```ip``` : show/manipulate routing, network devices, interfaces and tunnels
	- ```netstat``` : print network connections, routing tables, interface stats, masquerade connections, and multicast memberships
	- ```ss``` : investigate sockets
	- ```wget``` : retrieve files using HTTP, HTTPS, and FTP
		- ```wget https://website.com/<file>``` downloads a single file
		- ```wget -O <file-with-custom-name> https://website.com/<file>``` downloads a file and saves it with a new name
		- ```wget https://website.com/<file> https://website.com/<file>``` downloads multiple files
		- ```wget -b https://website.com/<large-file>``` downloads a file in the background
		- ```wget -c https://website.com/<large-file>``` continue an interrupted download
		- ```wget --user-agent="Mozilla/5.0" https://website.com/<file>``` download a file with a specific user agent
		- ```wget -i <txt_file>``` downloads files that are 'listed' in a txt file
		- ```wget --user=<user> --password=<password> https://website.com/private/<file>``` downloads a file with authentication
		- ```wget -P /path/to/directory https://website.com/<file>``` download a file to a specific directory
		- ```wget -e use_proxy=yes -e http_proxy=http://proxy.website.com:8080 https://website.com/<file>``` using wget commands with a proxy
	- ```curl``` : transfer data from or to a server

# Package Management:
	- ```apt-get``` : APT package handling utility
	- ```apt``` : command-line interface for the package management system

# Archiving and File Compression:
	- ```tar``` : tape archiver
	- ```gzip``` : compress or expand files
	- ```zip``` : package and compress files
	- ```unzip``` : list, test, and extract compressed files in a ZIP archive

# Text Processing:
	- ```awk``` : pattern scanning and processing language
	- ```sed``` : stream editor for filtering and transforming text
	- ```sort``` : sort lines of text files
	- ```uniq``` : report or omit repeated lines
	- ```wc``` : print newline, word, and byte counts for each file

# File Transfer:
	- ```scp``` : soft copy remote files
	- ```rysnc``` : fast, versatile, remote & local file-copying

# Miscellaneous Commands:
	- ```echo``` : display a line of text
	- ```date``` : print or set the system date and time
	- ```crontab``` : maintain crontab files for individual users
	- ```history``` : GNU history library
	- ```alias``` : define or display aliases
	- `xargs` : build and execute command lines from standard input
