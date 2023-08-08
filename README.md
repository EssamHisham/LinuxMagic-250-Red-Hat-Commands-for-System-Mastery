Mastering Linux Red Hat: 250 Essential Commands for Ultimate System Administration
# File and Directory Operations
## Listing and Navigation
ls [options] [directory]           # List directory contents
pwd                                # Print the current working directory
cd [directory]                     # Change the current directory

## Manipulation
mkdir [options] directory          # Create a new directory
rm [options] file/directory        # Remove files or directories
cp [options] source destination    # Copy files or directories
mv [options] source destination    # Move or rename files or directories

## Permissions and Ownership
chmod [options] permissions file   # Change file permissions
chown [options] owner:group file   # Change file ownership

# Process Management
ps [options]                       # Display information about running processes
top                                # Display dynamic view of system processes
htop                               # Interactive process viewer (enhanced 'top')

# Disk and Memory Usage
df [options]                       # Display disk space usage
du [options] file/directory        # Display file and directory space usage
free [options]                     # Display memory usage
vmstat                             # Display virtual memory statistics

# Text Processing
grep [options] pattern file        # Search for patterns in files
sed [options] 'commands' file      # Stream editor for text transformations

# File Compression and Archiving
## Archiving and Compression
tar [options] archive_file files   # Create archives and compress files
gzip [options] file                # Compress files
gunzip [options] file.gz           # Decompress files compressed with gzip
bzip2 [options] file               # Compress files using bzip2
unzip [options] file.zip           # Decompress files from a ZIP archive

# Package Management
yum [options] [command] [package]  # Package manager for Red Hat-based systems
dnf [options] [command] [package]  # Next-generation package manager

# System Services
## Managing Services
systemctl [options] [command] service  # Manage systemd services
service [options] service_name [start/stop/restart/status]  # Manage system services

# Firewall Management
firewall-cmd [options] [command]   # Manage firewall rules

# Network Configuration
## Network Interfaces
ifconfig                           # Display network interface information
ip [options] [command]             # Network configuration and IP management
nmcli [options] [command]          # NetworkManager command-line tool

## Routing and Networking
route [options]                    # Display or manipulate the routing table
netstat [options]                  # Display network connections, routing tables, interface statistics

# Network Testing
ping [options] host                # Test network connectivity to a host
traceroute [options] host          # Trace route to a host

# Remote Access
## Secure Shell (SSH)
ssh [options] user@host            # Secure shell remote login
scp [options] source destination   # Securely copy files between hosts

# File Synchronization
rsync [options] source destination # Remote file synchronization

# User Management
## Adding and Deleting Users
useradd [options] username         # Add a new user
userdel [options] username         # Delete a user

## User Authentication
passwd [options] username          # Change user password

# Disk Management
fdisk [options] device             # Partition table manipulator
parted [options] device            # Disk partition manipulator
mkfs [options] filesystem device  # Create a filesystem on a device
mount [options] device mount_point # Mount a filesystem
umount [options] mount_point       # Unmount a filesystem

# Software Installation
rpm [options] package.rpm          # Install or query RPM packages
yum groupinstall [options] group   # Install packages from package groups
dnf install [options] package      # Install packages using DNF

# Process Monitoring and Control
pkill [options] process_name       # Send signals to processes based on name
kill [options] PID                 # Send signals to processes based on PID
bg                                 # Place a job in the background
fg                                 # Bring a job to the foreground
nohup [command] &                  # Run a command that persists after the terminal session ends

# Logs and Monitoring
tail [options] log_file            # Output the last part of files
grep [options] pattern log_file    # Search for patterns in log files
journalctl [options]               # Query and display systemd journal logs
sar [options]                      # Collect and report system activity information

# System Information
uname [options]                    # Print system information
lsb_release [options]              # Print distribution-specific information
cat /etc/os-release                # Print operating system release information

# Date and Time
date [options]                     # Display or set the system date and time
timedatectl [options]              # Control the system time and date settings

# Archiving and Backup
rsnapshot [options]                # Filesystem snapshot utility
tar [options] archive_file files   # Create archives

# Software Repositories
yum repolist [options]             # List all enabled repositories
dnf repolist [options]             # List all enabled repositories using DNF

# Disk Quota Management
quotacheck [options]               # Scan filesystems for disk usage
quotaon [options]                  # Enable disk quotas
edquota [options] username         # Edit disk quotas for a user

# Kernel Management
uname [options]                    # Print kernel information
grubby [options]                   # Manage GRUB boot loader configuration
lsmod                              # List loaded kernel modules
modinfo [module]                   # Display information about a kernel module

# Network Services
netstat [options]                  # Print network connections, routing tables, interface statistics
lsof [options]                     # List open files and network connections
ss [options]                       # Socket statistics

# SSH Key Management
ssh-keygen [options]               # Generate SSH key pairs
ssh-copy-id [user]@[host]          # Copy SSH public key to remote host

# Cron Jobs
crontab [options]                  # Manage user cron jobs
cronie [options]                   # Manage cron jobs and configuration
systemctl [options] cron.service   # Manage the cron service

# User and Group Information
id [username]                      # Display user and group information
groups [username]                  # Display group memberships for a user
getent passwd                     # Display user account information from the user database
getent group                      # Display group information from the group database

# Environment Variables
env                                # Display environment variables
export [options] VARIABLE=value    # Set or modify environment variables

# Text Editors
vi [options] file                  # Open and edit files using vi
nano [options] file                # Open and edit files using nano

# Disk Usage Analysis
ncdu [options]                     # Interactively analyze disk usage
du [options] directory             # Estimate file and directory space usage

# Disk and Filesystem Health
smartctl [options] device          # Control and monitor SMART attributes of hard drives
fsck [options] device              # Check and repair a filesystem

# System Rescue and Recovery
init [options]                     # Change the system's runlevel
rescue.target                      # System rescue target for emergency mode

# System Updates
yum update [options]               # Update installed packages using yum
dnf upgrade [options]             # Upgrade installed packages using dnf

# SELinux Management
getenforce                         # Display SELinux enforcement mode
setenforce [Enforcing/Permissive]  # Change SELinux enforcement mode
sestatus                           # Display SELinux status
semanage [options]                 # Manage SELinux policies and configurations

# Network Bonding and Teaming
nmcli [options] connection add type bond/slave/... con-name [name]  # Add network connections
teamd [options]                    # Team network device driver management

# RAID Management
mdadm [options]                    # Manage RAID devices

# Shell Scripting
bash [script_file]                 # Run a Bash shell script
sh [script_file]                   # Run a shell script using the sh interpreter
chmod +x [script_file]             # Make a script executable

# DNS Configuration
dig [options] domain               # DNS lookup utility
nslookup [options] domain          # Query DNS servers for information

# Print Queues and Spooling
lp [options] file                  # Print files
lprm [options] job_id              # Remove print jobs from a queue

# Text Processing
awk '[pattern] { action }' file    # Text processing and reporting tool
cut [options] file                 # Remove sections from lines of files
sort [options] file                # Sort lines of text files
uniq [options] file                # Report or omit repeated lines

# File Searching
find [path] [expression]           # Search for files and directories
locate [options] pattern           # Find files using a prebuilt database
which [command]                    # Locate a command and display its path

# Network Connectivity
nmap [options] target              # Network exploration tool and security scanner
nc [options] host port             # Netcat - networking utility for reading/writing data across network connections

# SSL/TLS Certificate Management
openssl [options]                  # SSL/TLS toolkit
certbot [options]                  # Automatically obtain and install SSL/TLS certificates

# Container Management
docker [options]                   # Command-line interface for Docker containers
podman [options]                   # Command-line interface for Podman containers

# Compression and Archiving
xz [options] file                  # Compress or decompress .xz files
zip [options] file.zip files       # Create or extract ZIP archives

# Network Diagnostics
mtr [options] host                 # Network diagnostic tool
ssldump [options]                  # SSL/TLS network protocol analyzer

# Performance Monitoring
perf [options]                     # Linux performance analysis tool
sar [options]                      # Collect, report, or save system activity information

# Disk Encryption
cryptsetup [options]               # Manage disk encryption with dm-crypt and LUKS

# Network Time Protocol (NTP)
ntpdate [options]                  # Set the date and time via NTP
timedatectl [options] set-ntp [true/false]  # Enable or disable NTP synchronization

# Virtualization
qemu [options]                     # QEMU Emulator
virt-install [options]             # Create a virtual machine
virsh [options]                    # Command-line interface for managing virtual machines

# Sound Configuration
alsamixer                          # Text-based audio mixer
aplay [options] file               # Play audio files

# Memory Analysis
memtest86+ [options]               # Memory test tool

# RAID Management (mdadm)
mdadm [options]                    # Manage RAID devices

# System Backup
rsync [options] source destination # Remote file synchronization

# Remote Filesystem Access (NFS)
showmount [options]                # Show NFS shares
mount.nfs [options]                # Mount an NFS share

# Disk Cleanup
tmpwatch [options]                 # Remove files based on their age

# User and Group Management
groupadd [options] groupname       # Create a new group
groupdel [options] groupname       # Delete a group
gpasswd [options] groupname        # Modify group passwords

# Keyboard Configuration
loadkeys [options] keymap          # Load keyboard translation tables

# CPU Information
lscpu [options]                    # Display information about the CPU architecture

# USB Device Information
lsusb [options]                    # List USB devices

# System Clock Synchronization
ntpdate [options]                  # Set the date and time via NTP
timedatectl [options] set-ntp [true/false]  # Enable or disable NTP synchronization

# Swap Management
swapon [options] device            # Activate swap space
swapoff [options] device           # Deactivate swap space

# Software RAID (mdadm) Management
mdadm [options]                    # Manage RAID devices

# CPU Performance Scaling
cpupower [options]                 # Control CPU power and performance settings

# Memory Usage Monitoring
valgrind [options] program         # Memory usage analysis tool

# System Log Rotation
logrotate [options]                # Manage log files and their rotation

# System Maintenance
shutdown [options]                 # Shut down the system

# SELinux Troubleshooting
sealert [options]                  # SELinux alert browser and trouble report tool

# Authentication Configuration
authconfig [options]               # Configure system authentication services

# USB Device Management
usb_modeswitch [options]           # Activate USB devices

# Network Monitoring
tcpdump [options]                  # Dump network traffic

# Printer Management
system-config-printer [options]    # Configure printers

# IPv6 Configuration
ip6tables [options]                # Configure IPv6 firewall rules

# File Integrity Checking
aide [options]                     # Advanced Intrusion Detection Environment

# Remote Desktop
xrdp [options]                     # Remote desktop server

# User Interface
startx                             # Start X Window System

# Network Interface Bonding
modprobe [options] bonding         # Load the bonding kernel module
