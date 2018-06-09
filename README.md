# Data-Analysis-and-Tracking-Tool

This was a tool a wrote to do some data analysis of folders, open shares, simple data classification tagging.

Powershell Studio is needed to compile this, the .txt is just the raw code.




---------------------------------------------------------------------------------------------------------------------------------

Short Info:

*DFS Namespace is supported when searching by UNC
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Exports will be placed where the app is started in TXT format, please import them into excel as comma delimited -- enjoy

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Run with an account that has access to all your folders (domain admin, or make a special AD group and assign a new user). 
Use run-as OR login as user.
This possible could also be used to find everything group on shares/folders, or a regular user for some recon. Havn't tested it, but i dont see why not.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Classifications:
Empty groups in active directory used as 'tagging' for classifying folders.


Current Default Classification Groups:

Top Secret
Confidential
Private

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Data Discovery:
Requires the PowerShell AD module, and a domain user to query AD.
Select the OU to scan, this will iterate through each object in that OU.
I would also run this as a domain admin or a special user in a group that has local admin over servers.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Directory Analysis:
Root or recursive analysis of folders, either exports give information on folders ONLY, not files within.

Information in export: Folder Name, ACL, User Exists/Doesnt, Group Exists/Doesn't, Inherited/Not Inherited ACL

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------


File Analysis:
Recursively search selected folders for all files, export gives information to files ONLY.

Information in export: Folder Name, CreationTime, LastWrite, Owner, User Exists/Not, Group Exists/Not, Age of file(days)

--------------------------------------------------------------------------
![image](https://i.imgur.com/gwRNR6l.jpg)
![image](https://i.imgur.com/NbCxaho.jpg)
![image](https://i.imgur.com/tEMrJYZ.jpg)
![image](https://i.imgur.com/6ESgCSe.jpg)
![image](https://i.imgur.com/T2B9KOC.jpg)
![image](https://i.imgur.com/a1GDgrz.jpg)
