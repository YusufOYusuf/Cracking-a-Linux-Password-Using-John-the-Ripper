<h1>Cracking a Linux Password Using John the Ripper </h1>


<h2>Description</h2>
In this lab, I learned to crack a Linux password using John the Ripper. John the Ripper is a password cracker tool, which tries to detect weak passwords. It can also be used to recover passwords. You use John the Ripper to view the cracked passwords of a file named pwd.txt.
<br />



<h2>Environments Used </h2>

- <b>Kali GNU/Linux Rolling</b> 

<h2>Utilities and Language </h2>

- <b>Terminal</b>

<h2>Program walk-through:</h2>

<p align="center">
From the left sidebar, click Terminal and type the following commands: <br/>
1. unshadow /etc/passwd /etc/shadow > ~/Documents/pwd.txt <br/>
2. john --wordlist=~/Documents/crack.lst ~/Documents/pwd.txt <br/>
3. john --show ~/Documents/pwd.txt <br/>
<img src="https://i.postimg.cc/3N6RHBZp/Screen-Shot-2022-09-18-at-8-56-57-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
  
  
<br />
If the password cracked you will observe it displayed in the fortmat:<br/>
username:password:0:0:root:/root:/bin/bash <br/>
if you witness no password hash crack then it will display: <br/>
0 passwords hashes cracked <br/>
<img src="https://i.postimg.cc/3N6RHBZp/Screen-Shot-2022-09-18-at-8-56-57-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





