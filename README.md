# Creating-Users-with-PowerShell

Setup Remote Desktop for non-administrative users on Client-1
—
Log into Client-1 as mydomain.com\jane_admin
Open system properties
Click “Remote Desktop”
Allow “domain users” access to remote desktop
![image](https://github.com/user-attachments/assets/63792260-a27b-46aa-8587-dc9df1b836e1)

You can now log into Client-1 as a normal, non-administrative user now
Normally you’d want to do this with Group Policy that allows you to change MANY systems at once


Create a bunch of additional users and attempt to log into client-1 with one of the users
—
Login to DC-1 as jane_admin
Open PowerShell_ise as an administrator
Create a new File and paste the contents of the script into it
![image](https://github.com/user-attachments/assets/c44bd581-e15f-402d-904a-036e9b805d70)

Run the script and observe the accounts being created
![image](https://github.com/user-attachments/assets/9154922a-0f05-4580-a06c-a5ff44edfcce)

When finished, open ADUC and observe the accounts in the appropriate OU　(_EMPLOYEES)
![image](https://github.com/user-attachments/assets/dacc2037-90c5-43cc-84c3-cde59c7847f7)

attempt to log into Client-1 with one of the accounts (take note of the password in the script)
![image](https://github.com/user-attachments/assets/beddc031-f175-40d4-930a-1fcab49a55b1)

