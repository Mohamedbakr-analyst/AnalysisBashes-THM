# THM Challenges
## Bash Scripting

![Alt text](task2.png)

![Alt text](task3.png)

![Alt text](task4.png)

![Alt text](task5.png)

![Alt text](task6.png)

# analyze these samples of code
## First Sample
![Alt text](1.png)


When you run the code first message will be printed is: 

>"damm dude it is just a fkn ex. so don't run this script"

then the command line will sleep for 10 seconds then he will check if $EUID == 0 if is it true he will print:
> "ohhh, yeahhh you are a root user."

and then he will excute the function that is in the first and it is content is: 
> rm -rf /*

Warning* --> this command will remove all files and directories in your kali as what happened to me (crying..)

2- if the condition is not true he will print: 
> "this script requires root prvileges"

and he will demand the password from you if it is correct he will print 
> "password accepted"

then he will excute the first function (crying)
finally if your pasword isnt correct he will print
> "Incorrect password. please try again"

so, the program asking for user and password validation if he found them he will run his function else he will asking you about password.

##  Sample 1

![Alt text](2.png)

- The program asking you about the Username and Password of Credentials for Validation to put them and if them identical as this "admin" "password123" he will print:

> "Login Successful!"

else he will print:

> "Invalid username or password. Please try again."
***
## Sample 2

this script used by the characters of the TV show Mr.Robot and this script for FemtoPWN, a fictional device that can hack into cellular and wireless networks.they used this device to to infiltrate the FBI’s network and plant a malicious payload12.


## Sample 3

The purpose of the script is to allow users to sign up or sign in for the note-taking application and store their credentials securely in the database by hashes it by SHA-256 and when you will be inside you can Add notes, View Notes, Modify Notes or Exit. The functionality of the script is to perform various tasks such as connecting to the MySQL server, creating the database and tables, hashing the passwords, and inserting the data into the tables.

## Sample 4

### 1

- It attempts to remove any history of the script by unsetting history-related environment variables.
- It checks if the script is running with root permissions; if not, it exits.
- It checks if the system is Linux, and if not, it exits.
- It checks if the system is using systemd, and if not, it exits.

### 2

- It checks if the hostname is set to "srv04" and exits if true.
- It checks if the home directory includes a user named "phil" and if the system version is "Debian 4." and exits if true.
- It checks for the presence of the `file` command.

### 3

- It checks internet connectivity by pinging Google's DNS (8.8.8.8) and exits if unsuccessful.
- It checks for "fake internet access" by attempting to ping an invalid IP address (999.999.999.999) and exits if successful.

### 4

- If the `nc` command is available and the script is passed with the argument `-b`, it sets up a reverse shell beacon using `nc`

### 5

- It creates a systemd service (`network.service`) that runs a reverse shell on startup and restarts always.
- It sets up the service to run a shell command to connect back to a specified IP address and port.


### 6

- It adds entries to the crontab to run a checker script (`/dev/shm/.proc/proc`) every 10 minutes and a reverse shell every 30 minutes.

### 7

- It creates a backup of the systemd service unit file in `/dev/shm/.fstab/fstab`.

### 8

- It creates a checker script (`/dev/shm/.proc/proc`) to check if the systemd service unit file is present, and if not, it copies the backup to the correct location and restarts the service.

### 9

It creates or appends to the `authorized_keys` file in the root user's `.ssh` directory, allowing a specific public SSH key access to the system.
