# ZeroX
NOTE: Im not the creator of this trojan.So me and the cretor we aren't responsable for any damage

# Author notes:
Zero is my first PE infection virus. The name is from a Rockman character.

This is not overwriting virus!
The virus search for executable files to infect in the user profile. The virus also infect removable and network drives.

The file is infected by adding a new section that contains the virus code and the whole body of the virus itself. The virus body in the infected file is encrypted.

# Features:
1) Infects files in user profile, removable and network drives.

2) Infects file by adding new section to the file.

3) The virus body in the infected file is encrypted.

4) Anti-debugging.

5) Run on Windows startup.

6) Multithreaded.

7) Uses Native API.

 

When an infected file is executed, it performs the following actions:

 

1) The virus code executes, and parse the loader data from the PEB to resolve all APIs that the virus code needs.

2) The virus code drop the virus executable in the temp folder.

3) The virus executable is executed, and the virus installs itself to the system.

4) The original entry point of the infected file is called, and the program runs as normal.

# ZeroX 
# New Features :
This is the rewrite version of my old Zero virus with some improvement.

# New features:

1.DLL infection
2.The virus body in the infected file is now encrypted with RC4. The timestamp value of the target file is used as encryption key, which is 32 bits (4 bytes) long
3.Deletes non PE files
4.Crash the operating system every a hour
5.uses Unicode, so the virus can infect files that has Unicode characters in their filename, such as Japanese
