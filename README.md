# XDBInfo 1.0.0.5
XDBInfo.exe is an application designed to perform automatic backups of Firebird databases and send notifications via Telegram. This guide will help users understand how to configure and use the application effectively."


# Features
Compresses daily backup files automatically into ZIP format
Generates restore reports to confirm that backups are valid
Creates separate log files for backup and restore processes
Sending notifications to Telegram regarding the status of the database, whether it encounters issues or operates successfully.
Providing information about the remaining storage capacity on connected computers.


# Installation
System Requirements

- Windows operating system
- Firebird (Full Installation)
- Internet connection for telegram notifications

# Installation Steps
Download and extract the XDBInfo.exe file to your desired directory.
Ensure that Firebird is installed and accessible from the system.
Edit the config.ini configuration file as needed (see the next section).
Run XDBInfo.exe through Windows Task Scheduler with the Run with highest privileges option.
Application Configuration
The application uses the config.ini file to store configuration parameters.

# Parameter Descriptions ( config.ini )

- gbak_path – Path to the gbak.exe executable used for database backup.
- database_folder – Directory where the databases are located.
- backup_folder – Location to store backup files.
- max_backup_files – Maximum number of backup files to keep before older ones are deleted.
- database_list – List of databases to be backed up.
- bot_token – API telegram @BotFather.
- chat_id – Chat ID from telegram bot.

Using the Application
Running the Backup Run XDBInfo.exe. The application will automatically back up the databases listed in config.ini.

# Receiving Notifications
Once the backup is complete, the user will receive an telegram notification.

# Checking the Log
The application generates a detailed log for each backup process. Check the backup.log file for more information.

# Conclusion
This guide is intended to help users understand how XDBInfo.exe works and how to optimize the database backup process. Ensure the configuration file is correctly set up so the system runs smoothly.
