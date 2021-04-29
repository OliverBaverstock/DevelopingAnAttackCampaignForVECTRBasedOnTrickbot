README

Uncompiled Folder:
	- This contains the source code without being compiled

Compiled Folder:
	- This contains compiled code ready to be run
	- Also contains campaign to import into VECTR

To Run:
	- DO NOT RUN ON YOUR HOST MACHINE(This is a virus/malware)

	- Set up Virtual Environment/Network in VMware or VirtualBox

	- Attacker Machine
		- Preferably a Kali Linux Machine
		- Give machine IP address 10.42.0.1
		- Add C2 file onto this machine
		- Run requirements.txt within C2 folder
		- Run C2 Server with python3 c2.py
			- Start listener(Use help command for instructions)
			- Instructions also at https://github.com/0xRick/c2
		- Start an apache server
			- sudo service apache2 start
		- Put MessageDLL.dll and malFile onto Apache server
			- Into /var/www/html/
		- Ensure above files have 766 permission with "ls -la"
			- If not use "chmod 766 filename"
	
	- VECTR Machine
		- Install VECTR on Ubuntu machine
		- Instructions at https://docs.vectr.io/Installation/
		- Import campaign provided in compiled folder
		- Start test cases as desired

	- Victim Machine
		- Windows VM
		- Execute Word Document on the victim machine

Note:
	- If files get removed from machine for being flagged as malicious contact me at oliverbaverstock@yahoo.ie or redownload
		