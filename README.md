
# `sysopctl` TOOL GUIDE

**Version:** v0.1.0

## Introduction

`sysopctl` is a versatile command-line utility built to streamline system management tasks. It offers a user-friendly interface that helps administrators handle essential operations such as managing system services, tracking and analyzing system processes, reviewing logs, and performing backups. By combining features found in tools like `systemctl`, `uptime`, `df`, `top`, `journalctl`, and `rsync`, sysopctl consolidates several system administration functions into a single, efficient tool, making it easier to perform routine tasks with minimal effort.

## How To Use
Each command in sysopctl follows this structure:

```
sysopctl <command> [options]
```

<!-- Installation of Sysopctl -->

### Basic Commands

#### 1. View Manual 
To view the complete documentation using the manual page:

```
man sysopctl
```
![man](https://github.com/user-attachments/assets/493127b3-aa9c-4b61-bb18-4579456ac8c1)

#### 2. Help Menu
To display a list of commands and examples for using sysopctl:

```
sysopctl --help
```
![help](https://github.com/user-attachments/assets/17bdae92-aee4-49e8-96f9-ff1fdee81f51)


#### 3. Version Information
To check which version of `sysopctl` you have installed:

```
sysopctl --version
```
![version](https://github.com/user-attachments/assets/4360be1a-e911-4b5a-bc73-d1bc62518db7)


### System Management Commands

#### Part 1: Beginner Level Operation

##### 1. List Active Services
Retrieve a list of currently running services, similar to `systemctl list-units --type=service`.

**Command:**
```
sysopctl service list
```
![service list](https://github.com/user-attachments/assets/dde93664-0526-41e7-a6d1-486a1701b9f6)


##### 2. Check System Load
Shows the system's load averages, similar to what `uptime` displays.

**Command:**
```
sysopctl system load
```
![system load](https://github.com/user-attachments/assets/81253e36-a861-4459-b5b8-0559c287dc7d)


#### Part 2: Intermediate Level

##### 1. Service Management
Starts or stops a specific service, comparable to  `systemctl start/stop`.


**Start a Service:**
```
sysopctl service Start <service-name>
```
**Stop a Service:**
```
sysopctl service stop <service-name>
```
![stop service](https://github.com/user-attachments/assets/3248a52c-1924-4545-a264-a0e8b0fc94aa)



##### 2. Check Disk Usage
View the disk usage of mounted partitions, similar to `df -h`.

**Command:**
```
sysopctl disk usage
```
![disk usage](https://github.com/user-attachments/assets/6f088e67-3c88-4560-9866-0a63de835a4d)


#### Part 3: Advanced Level

##### 1. Monitor System Processes
Track Real Time Activity, similar to using `top` or `htop`.

**Command:**
```
sysopctl process monitor
```
![Screenshot from 2024-09-11 15-34-39](https://github.com/user-attachments/assets/873cead7-085c-4953-bf3a-8eddb32eace2)



##### 2. Log Analysis
Review and summarize important recent logs, much like `journalctl`.

**Command:**
```
sysopctl logs analyse
```
![logs](https://github.com/user-attachments/assets/00e00828-f457-498f-9281-8dd1aff30db8)


##### 3. Backup System Data
Backup designated files or directories using a command similar to `rsync`.

**Command:**
```
sysopctl backup <path>
```
![backup](https://github.com/user-attachments/assets/5d5bdd4e-5edb-43f3-a6a1-9342b726a5d5)



