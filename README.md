# My-Ethicalhacking-projects
As a passionate Software Engineer and un Ethical hacker, this repository will be containing my hacking projects. 
I am Mwesigye Nicholas I graduated as un orthopeadic medical clinicial from Mugalo paramedical school Uganda, but as I continued with this journey I realised that technology was holding the future
from then I decided to enter tech and my goal from then was to be the best version of myself in Ethical hacking and software engineering.
growing in a third world country where techology is just developing, demand for software engineers increasing and cyber-attacks increasing I decided to specialise in these two areas 
so as to design customised software and protect my country against cyber-attacks

I build my hacking lab containing metasploitable2, windows 10 xp, kali and parrot machines.
I will be starting my hacking project with exploiting the metasploitable2 machine.

STEP 1:
I started by attacking the smtp protocol running on port 25 on my target machine.
I started by pinging the target machine to see whether the machine is up.

![project image 1](https://github.com/Mwesigye-Nicholas/My-Ethicalhacking-projects/assets/111627142/a022eaa5-3426-4768-845f-ec7b74d62667)

STEP 2:
Scanning the target machine targetting specifically port 25 to confirm that its running smtp because sometime misconfigurations can occur.
![project image 2](https://github.com/Mwesigye-Nicholas/My-Ethicalhacking-projects/assets/111627142/fd39de75-cf73-46b0-b58f-1138256eeb10)

STEP 3:
Now we open up our metasploit frame.
![project image 3](https://github.com/Mwesigye-Nicholas/My-Ethicalhacking-projects/assets/111627142/f6a162cf-c0f5-459e-b48c-1f0c04a86589)

scanning can also be done by using auxiliary module scanner for smtp in metasploit
![project image 4](https://github.com/Mwesigye-Nicholas/My-Ethicalhacking-projects/assets/111627142/efc09cf8-21c8-457a-8074-27d622f23eb0)

STEP 4:
Now i search the smtp specific scripts in the auxiliary module
![project image 5](https://github.com/Mwesigye-Nicholas/My-Ethicalhacking-projects/assets/111627142/c935b5df-2bdf-478c-bcfc-a12fa5eaa202)

STEP 5:
Then we use the smtp_enum which allows us to enumerate users which is located on number 25 and we setup the missing arguments and run the run the module which connects to metasploitable2 machine.
![project image 6](https://github.com/Mwesigye-Nicholas/My-Ethicalhacking-projects/assets/111627142/444b2568-7f03-40d3-b3e6-15efb03ab260)

STEP 6:
I open up another terminal and use the netcat(nc) command which help us establish connection,followed the ip address of the target and the port machine its listening the service on .smtp uses some commands on of which is the VRFY command that allows use to verify users, we verify one which turn to be in the target machine database and the Nicholas that turns out not to be.
