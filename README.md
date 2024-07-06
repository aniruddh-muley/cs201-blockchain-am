# cs201-blockchain-am

## Description:
A very basic voting system implemented as part of a course project, to demonstrate the utility of blockchains.<br />
The voting system is in the form of an interactive menu, with the option to view the candidates, register as a voter, and cast your vote. You can only cast one vote, only to a valid candidate, and only once with a registered ID.<br />
There is also an option to access what's beneath the hood using admin controls, upon entering the correct password. This allows the admin to generate the election blockchain, tally the votes and declare the winner, and examine the blockchain itself.<br />
The bc_vot_sys.cpp file, which is the code for the blockchain based voting system, needs to be compiled using OpenSSL. OpenSSL needs to be installed in the user's computer before execution, otherwise the code won't run. After installing OpenSSL, the user needs to update the includePath with the include folder path of the OpenSSL directory.<br />
Let's say that OpenSSL has been installed at the following address: "C:\Program Files\OpenSSL-Win64". Hence, for a Windows user, the file can be compiled like this, using Command Prompt:<br />
```
g++ -c bc_vot_sys.cpp -I"C:\Program Files\OpenSSL-Win64\include"
g++ bc_vot_sys.o -o bc_vot_sys.exe -L"C:\Program Files\OpenSSL-Win64\lib" -lssl -lcrypto
bc_vot_sys.exe
```

Upon execution, the user will get a menu interface, and needs to enter the appropriate options/commands to proceed and run the program. A test case has been given in bc_testcase.txt.
