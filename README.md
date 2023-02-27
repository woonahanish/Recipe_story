# CS5346_P1
Computer expert system to identify the type of the network attacks and possible preventions.

To Run the program use a suitable c++ compiler to convert DecTree_complete.cpp into a execuitable file, then run the .exe file.

Rules - Backward

10 if PROBLEM = NO
	Then ATTACK = NO
20 if PROBLEM = YES
	Then ATTACK = YES
30 if SLOW = YES AND
	ATTACK = YES
	Then ATTACK ACTIVE = YES
40 if SLOW = YES AND
	ATTACK = NO
	Then ATTACK ACTIVE = NO
50 if ATTACK = YES AND
	ATTACK ACTIVE = YES
	Then ATTACK TYPE = YES
60 if ATTACK TYPE = YES AND
	SLOW = YES AND
	UNNECESSARY PROCESSOR RUNNING = YES
	Then ATTACK TYPE M = YES
70 if ATTACK TYPE = YES AND
	UNNECESSARY PROCESSOR RUNNING = YES AND
	NO RESPONSE = YES
	Then ATTACK TYPE D = YES
80 if ATTACK TYPE = YES AND
	UNNECESSARY PROCESSOR RUNNING = YES AND
	UNKNOWN FILES = YES
	Then ATTACK TYPE MAL = YES 
90 if ATTACK TYPE = YES AND
	SLOW = YES AND
	NO RESPONSE = YES
	Then ATTACK = NO
100 if 	UNKNOWN FILES = YES AND
	UNAUTHORIZED ACTIVITY = YES AND
	UNKNOWN EMAILS = YES	
Then ATTACKTYPE ID  = YES
110 if ACTIVE ATTACK = YES AND
	FLOODING REQUEST = YES AND
	CRASHED SYSTEM = YES
	Then ATTACK TYPE DENH= YES
120 if ACTIVE ATTACK = YES AND
	UNNECESSARY PROCESSOR RUNNING = YES AND
	PASSWARD COMPROMISED = YES
	Then ATTACK TYPE IDH= YES
130 if ACTIVE ATTACK = YES AND
	FLOODING REQUEST = YES AND
	CRASHED SYSTEM = NO
	Then ATTACK TYPE DENN = YES
140 if ACTIVE ATTACK = YES AND
	PASSWARD COMPROMISED = YES AND
	UNKNOWN FILE = YES
	Then ATTACK TYPE IDH= YES
150 if ACTIVE ATTACK = YES AND
	PASSWARD COMPROMISED = YES AND
	UNKNOWN FILE = NO
	Then ATTACK TYPE IDHN= YES
160 if PROBLEM = YES AND
	SLOW = YES AND
	NO RESPONSE = YES
	Then ATTACK TYPE P= YES
170 if PROBLEM = YES AND
	SLOW = YES AND
	LOST FILES = YES
	Then ATTACK TYPE M= YES
180 if PROBLEM = YES AND
	SLOW = YES AND
	UNNECESSARY PROCESSOR RUNNING = NO
	Then ATTACK TYPE ACTIVE= NO
190 if ATTACK TYPE= YES AND
	SLOW = NO AND
	PASSWARD COMPROMISED = YES
	Then ATTACK  TYPE ID P= YES
200 if PROBLEM = YES AND
	BUG = YES AND
	CRASHED SYSTEM = YES
	Then ATTACK TYPE MAL Y= YES



![back](https://user-images.githubusercontent.com/25388169/221639239-a901d24c-7c92-4374-9985-5903e333852f.jpg)

Rules - Forward

'10' IF BasicAttack=true THEN Install antivirus software.
'20' IF IdentityAttack=true THEN Use a VPN.
'30' IF DenialOfService=true THEN Have multilevel authentication for users.
'40' IF MaliciousCode=true THEN Don't download any files from unknown source. 
'50' IF PasswordAttack=true THEN Use stronger password.
'60' IF PhishingAttack=true THEN Implement email filter from unknown source.
'70' IF ManInTheMiddle=true THEN Use encryption.


![Flowchart-2](https://user-images.githubusercontent.com/48315412/221670612-1c2b00f5-c06a-4f4a-aca6-c67507c88f6f.png)


