# Checks-disk-usage-script

The script checks the usage of the root partition on a Linux system and sends an email warning if the usage is greater than or equal to 20%. 

The script performs the following steps:

1. It gets the disk usage information for the root partition using the df command.
2. It filters out all lines except the one for the root partition using grep.
3. It extracts the usage percentage using awk.
4. It checks if the usage is greater than or equal to 20%.
5. If the usage is greater than or equal to 20%, it sends an email to the specified email address containing the warning message, which includes the disk usage percentage and the current date and time.
