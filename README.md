<h2>SYSTEM INFORMATION</h2> 
<p># Display Linux system information</p> 
<h4>uname -a</h4>
<p># Display kernel release information</p>
<h4>uname -r</h4>
<p># Show which version of redhat installed</p> 
<h4>cat /etc/redhat-release</h4> 
<p># Show how long the system has been running + load </p>
<h4>uptime</h4> 
<p># Show system host name</p> 
<h4>hostname</h4> 
<p># Display the IP addresses of the host</p> 
<h4>hostname -I</h4> 
<p># Show system reboot history</p> 
<h4>last reboot</h4> 
<p># Show the current date and time</p> 
<h4>date</h4> 
<p># Show this month's calendar</p> 
<h4>cal</h4> 
<p># Display who is online</p> 
<h4>w</h4> 
<p># Who you are logged in as</p>
<h4>whoami</h4>


<h2>HARDWARE INFORMATION</h2>
<p># Display messages in kernel ring buffer</p>
<h4>dmesg</h4>
<p># Display CPU information</p>
<h4>cat /proc/cpuinfo</h4>
<p># Display memory information</p>
<h4>cat /proc/meminfo</h4>
<p># Display free and used memory ( -h for human readable, -m for MB, -g for GB.)</p>
<h4>free -h</h4>
<p># Display PCI devices</p>
<h4>lspci -tv</h4>
<p># Display USB devices</p>
<h4>lsusb -tv</h4>
<p># Display DMI/SMBIOS (hardware info) from the BIOS</p>
<h4>dmidecode</h4>
<p># Show info about disk sda</p>
<h4>hdparm -i /dev/sda</h4>
<p># Perform a read speed test on disk sda</p>
<h4>hdparm -tT /dev/sda</h4>
<p># Test for unreadable blocks on disk sda</p>
<h4>badblocks -s /dev/sda</h4>


<h2>PERFORMANCE MONITORING AND STATISTICS</h2>
<p># Display and manage the top processes</P>
<h4>top</h4>
<p># Interactive process viewer (top alternative)</P>
<h4>htop</h4>
<p># Display processor related statistics</P>
<h4>mpstat 1</h4>
<p># Display virtual memory statistics</P>
<h4>vmstat 1</h4>
<p># Display I/O statistics</P>
<h4>iostat 1</h4>
<p># Display the last 100 syslog messages  (Use /var/log/syslog for Debian based systems.)</P>
<h4>tail 100 /var/log/messages</h4>
<p># Capture and display all packets on interface eth0</P>
<h4>tcpdump -i eth0</h4>
<p># Monitor all traffic on port 80 ( HTTP )</P>
<h4>tcpdump -i eth0 'port 80'</h4>
<p># List all open files on the system</P>
<h4>lsof</h4>
<p># List files opened by user</P>
<h4>lsof -u user</h4>
<p># Display free and used memory ( -h for human readable, -m for MB, -g for GB.)</P>
<h4>free -h</h4>
<p># Execute "df -h", showing periodic updates</P>
<h4>watch df -h</h4>


<h2>USER INFORMATION AND MANAGEMENT</h2>
<p># Display the user and group ids of your current user.</p>
<h4>id</h4>
<p># Display the last users who have logged onto the system.</p>
<h4>last</h4>
<p># Show who is logged into the system.</p>
<h4>who</h4>
<p># Show who is logged in and what they are doing.</p>
<h4>w</h4>
<p># Create a group named "test".</p>
<h4>groupadd test</h4>
<p># Create an account named john, with a comment of "John Smith" and create the user's home directory.</p>
<h4>useradd -c "John Smith" -m john</h4>
<p># Delete the john account.</p>
<h4>userdel john</h4>
<p># Add the john account to the sales group</p>
<h4>usermod -aG sales john</h4>


<h2>FILE AND DIRECTORY COMMANDS</h2>
<p># List all files in a long listing (detailed) format</p>
<h4>ls -al</h4>
<p># Display the present working directory</p>
<h4>pwd</h4>
<p># Create a directory</p>
<h4>mkdir directory</h4>
<p># Remove (delete) file</p>
<h4>rm file</h4>
<p># Remove the directory and its contents recursively</p>
<h4>rm -r directory</h4>
<p># Force removal of file without prompting for confirmation</p>
<h4>rm -f file</h4>
<p># Forcefully remove directory recursively</p>
<h4>rm -rf directory</h4>
<p># Copy file1 to file2</p>
<h4>cp file1 file2</h4>
<p># Copy source_directory recursively to destination. If destination exists, copy source_directory into destination, otherwise create destination with the contents of source_directory.</p>
<h4>cp -r source_directory destination</h4>
<p># Rename or move file1 to file2. If file2 is an existing directory, move file1 into directory file2</p>
<h4>mv file1 file2</h4>
<p># Create symbolic link to linkname</p>
<h4>ln -s /path/to/file linkname</h4>
<p># Create an empty file or update the access and modification times of file.</p>
<h4>touch file</h4>
<p># View the contents of file</p>
<h4>cat file</h4>
<p># Browse through a text file</p>
<h4>less file</h4>
<p># Display the first 10 lines of file</p>
<h4>head file</h4>
<p># Display the last 10 lines of file</p>
<h4>tail file</h4>
<p># Display the last 10 lines of file and "follow" the file as it grows.</p>
<h4>tail -f file</h4>


<h2>PROCESS MANAGEMENT</h2>
<p># Display your currently running processes</p>
<h4>ps</h4>
<p># Display all the currently running processes on the system.</p>
<h4>ps -ef</h4>
<p># Display process information for processname</p>
<h4>ps -ef | grep processname</h4>
<p># Display and manage the top processes</p>
<h4>top</h4>
<p># Interactive process viewer (top alternative)</p>
<h4>htop</h4>
<p># Kill process with process ID of pid</p>
<h4>kill pid</h4>
<p># Kill all processes named processname</p>
<h4>killall processname</h4>
<p># Start program in the background</p>
<h4>program &</h4>
<p># Display stopped or background jobs</p>
<h4>bg</h4>
<p># Brings the most recent background job to foreground</p>
<h4>fg</h4>
<p># Brings job n to the foreground</p>
<h4>fg n</h4>


<h2>NETWORKING</h2>
<p># Display all network interfaces and ip address</p>
<h4>ifconfig -a</h4>
<p># Display eth0 address and details</p>
<h4>ifconfig eth0</h4>
<p># Query or control network driver and hardware settings</p>
<h4>ethtool eth0</h4>
<p># Send ICMP echo request to host</p>
<h4>ping host</h4>
<p># Display whois information for domain</p>
<h4>whois domain</h4>
<p># Display DNS information for domain</p>
<h4>dig domain</h4>
<p># Reverse lookup of IP_ADDRESS</p>
<h4>dig -x IP_ADDRESS</h4>
<p># Display DNS ip address for domain</p>
<h4>host domain</h4>
<p># Display the network address of the host name.</p>
<h4>hostname -i</h4>
<p># Display all local ip addresses</p>
<h4>hostname -I</h4>
<p># Download http://domain.com/file</p>
<h4>wget http://domain.com/file</h4>
<p># Display listening tcp and udp ports and corresponding programs</p>
<h4>netstat -nutlp</h4>


<h2>ARCHIVES (TAR FILES)</h2>
<p># Create tar named archive.tar containing directory.</p>
<h4>tar cf archive.tar directory</h4>
<p># Extract the contents from archive.tar.</p>
<h4>tar xf archive.tar</h4>
<p># Create a gzip compressed tar file name archive.tar.gz.</p>
<h4>tar czf archive.tar.gz directory</h4>
<p># Extract a gzip compressed tar file.</p>
<h4>tar xzf archive.tar.gz</h4>
<p># Create a tar file with bzip2 compression</p>
<h4>tar cjf archive.tar.bz2 directory</h4>
<p># Extract a bzip2 compressed tar file.</p>
<h4>tar xjf archive.tar.bz2</h4>


<h2>INSTALLING PACKAGES</h2>
<p># Search for a package by keyword.</p>
<h4>yum search keyword</h4>
<p># Install package.</p>
<h4>yum install package</h4>
<p># Display description and summary information about package.</p>
<h4>yum info package</h4>
<p># Install package from local file named package.rpm</p>
<h4>rpm -i package.rpm</h4>
<p># Remove/uninstall package.</p>
<h4>yum remove package</h4>
<p># Install software from source code.</p>
<h4>tar zxvf sourcecode.tar.gz</br>
cd sourcecode</br>
./configure</br>
make</br>
make install</h4>


<h2>SEARCH</h2>
<p># Search for pattern in file</p>
<h4>grep pattern file</h4>
<p># Search recursively for pattern in directory</p>
<h4>grep -r pattern directory</h4>
<p># Find files and directories by name</p>
<h4>locate name</h4>
<p># Find files in /home/john that start with "prefix".</p>
<h4>find /home/john -name 'prefix*'</h4>
<p># Find files larger than 100MB in /home</p>
<h4>find /home -size +100M</h4>


<h2>SSH LOGINS</h2>
<p># Connect to host as your local username.</p>
<h4>ssh host</h4>
<p># Connect to host as user</p>
<h4>ssh user@host</h4>
<p># Connect to host using port</p>
<h4>ssh -p port user@host</h4>


<h2>FILE TRANSFERS</h2>
<p># Secure copy file.txt to the /tmp folder on server</p>
<h4>scp file.txt server:/tmp</h4>
<p># Copy *.html files from server to the local /tmp folder.</p>
<h4>scp server:/var/www/*.html /tmp</h4>
<p># Copy all files and directories recursively from server to the current system's /tmp folder.</p>
<h4>scp -r server:/var/www /tmp</h4>
<p># Synchronize /home to /backups/home</p>
<h4>rsync -a /home /backups/</h4>
<p># Synchronize files/directories between the local and remote system with compression enabled</p>
<h4>rsync -avz /home server:/backups/</h4>


<h2>DISK USAGE</h2>
<p># Show free and used space on mounted filesystems</p>
<h4>df -h</h4>
<p># Show free and used inodes on mounted filesystems</p>
<h4>df -i</h4>
<p># Display disks partitions sizes and types</p>
<h4>fdisk -l</h4>
<p># Display disk usage for all files and directories in human readable format</p>
<h4>du -ah</h4>
<p># Display total disk usage off the current directory</p>
<h4>du -sh</h4>


<h2>DIRECTORY NAVIGATION</h2>
<p># To go up one level of the directory tree.  (Change into the parent directory.)</p>
<h4>cd ..</h4>
<p># Go to the $HOME directory</p>
<h4>cd</h4>
<p># Change to the /etc directory</p>
<h4>cd /etc</h4>
