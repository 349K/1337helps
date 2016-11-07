<p><b>Kernel, Operating System &amp; Device Information:</b></p>
<table width="700px">
   <tbody>
      <tr>
         <th style="width:40%"><b>Command</b></th>
         <th><b>Result</b></th>
      </tr>
      <tr>
         <td><code>uname -a</code></td>
         <td>Print all available system information</td>
      </tr>
      <tr>
         <td><code>uname -r</code></td>
         <td>Kernel release</td>
      </tr>
      <tr>
         <td><code>uname -n</code></td>
         <td>System hostname</td>
      </tr>
      <tr>
         <td><code>hostname</code></td>
         <td>As above</td>
      </tr>
      <tr>
         <td><code>uname -m</code></td>
         <td>Linux kernel architecture (32 or 64 bit)</td>
      </tr>
      <tr>
         <td><code>cat /proc/version</code></td>
         <td>Kernel information</td>
      </tr>
      <tr>
         <td><code>cat /etc/*-release</code></td>
         <td>Distribution information</td>
      </tr>
      <tr>
         <td><code>cat /etc/issue</code></td>
         <td>As above</td>
      </tr>
      <tr>
         <td><code>cat /proc/cpuinfo</code></td>
         <td>CPU information</td>
      </tr>
      <tr>
         <td><code>df -a</code></td>
         <td>File system information</td>
      </tr>
   </tbody>
</table>
<p>&nbsp;</p>
<p><b>Users &amp; Groups:</b></p>
<table width="700px">
   <tbody>
      <tr>
         <th style="width:40%"><b>Command</b></th>
         <th><b>Result</b></th>
      </tr>
      <tr>
         <td><code>cat /etc/passwd</code></td>
         <td>List all users on the system</td>
      </tr>
      <tr>
         <td><code>cat /etc/group</code></td>
         <td>List all groups on the system</td>
      </tr>
      <tr>
         <td><code>for i in $(cat /etc/passwd 2&gt;/dev/null| cut -d":" -f1 2&gt;/dev/null);do id $i;done 2&gt;/dev/null</code></td>
         <td>List all uid’s and respective group memberships</td>
      </tr>
      <tr>
         <td><code>cat /etc/shadow</code></td>
         <td>Privileged command</td>
      </tr>
      <tr>
         <td><code>grep -v -E "^#" /etc/passwd | awk -F: '$3 == 0 { print $1}'</code></td>
         <td>List all super user accounts</td>
      </tr>
      <tr>
         <td><code>finger</code></td>
         <td>Users currently logged in</td>
      </tr>
      <tr>
         <td><code>pinky</code></td>
         <td>As above</td>
      </tr>
      <tr>
         <td><code>users</code></td>
         <td>As above</td>
      </tr>
      <tr>
         <td><code>who -a</code></td>
         <td>As above</td>
      </tr>
      <tr>
         <td><code>w</code></td>
         <td>Who is currently logged in and what they’re doing</td>
      </tr>
      <tr>
         <td><code>last</code></td>
         <td>Listing of last logged on users</td>
      </tr>
      <tr>
         <td><code>lastlog</code></td>
         <td>Information on when all users last logged in</td>
      </tr>
      <tr>
         <td><code>lastlog –u %username%</code></td>
         <td>Information on when the specified user last logged in</td>
      </tr>
      <tr>
         <td><code>lastlog |grep -v "Never"</code></td>
         <td>Entire list of previously logged on users</td>
      </tr>
   </tbody>
</table>
<p>&nbsp;</p>
<p></p>
<p><b>User &amp; Privilege Information:</b></p>
<table width="700px">
   <tbody>
      <tr>
         <th style="width:40%"><b>Command</b></th>
         <th><b>Result</b></th>
      </tr>
      <tr>
         <td><code>whoami</code></td>
         <td>Current username</td>
      </tr>
      <tr>
         <td><code>id</code></td>
         <td>Current user information</td>
      </tr>
      <tr>
         <td><code>cat /etc/sudoers</code></td>
         <td>Privileged command</td>
      </tr>
      <tr>
         <td><code>sudo -l</code></td>
         <td>Can the current user perform anything as root</td>
      </tr>
      <tr>
         <td><code>sudo -l 2&gt;/dev/null | grep -w 'nmap|perl|'awk'|'find'|'bash'|'sh'|'man'<br>|'more'|'less'|'vi'|'vim'|'nc'|'netcat'|python<br>|ruby|lua|irb' | xargs -r ls -la 2&gt;/dev/null</code></td>
         <td>Can the current user run any ‘interesting’ binaries as root and if so also display the binary permissions etc.</td>
      </tr>
   </tbody>
</table>
<p>&nbsp;</p>
<p><b>Environmental Information:</b></p>
<table width="700px">
   <tbody>
      <tr>
         <th style="width:40%"><b>Command</b></th>
         <th><b>Result</b></th>
      </tr>
      <tr>
         <td><code>env</code></td>
         <td>Display environmental variables</td>
      </tr>
      <tr>
         <td><code>set</code></td>
         <td>As above</td>
      </tr>
      <tr>
         <td><code>echo $PATH</code></td>
         <td>Path information</td>
      </tr>
      <tr>
         <td><code>history</code></td>
         <td>Displays command history of current user</td>
      </tr>
      <tr>
         <td><code>pwd</code></td>
         <td>Print working directory, i.e. ‘where am I’</td>
      </tr>
      <tr>
         <td><code>cat /etc/profile</code></td>
         <td>Display default system variables</td>
      </tr>
      <tr>
         <td><code>cat /etc/shells</code></td>
         <td>Display available shells</td>
      </tr>
   </tbody>
</table>
<p>&nbsp;</p>
<p><b>Interesting Files:</b></p>
<table width="700px">
   <tbody>
      <tr>
         <th style="width:40%"><b>Command</b></th>
         <th><b>Result</b></th>
      </tr>
      <tr>
         <td><code>find / -perm -4000 -type f 2&gt;/dev/null</code></td>
         <td>Find SUID files</td>
      </tr>
      <tr>
         <td><code>find / -uid 0 -perm -4000 -type f 2&gt;/dev/null</code></td>
         <td>Find SUID files owned by root</td>
      </tr>
      <tr>
         <td><code>find / -perm -2000 -type f 2&gt;/dev/null</code></td>
         <td>Find GUID files</td>
      </tr>
      <tr>
         <td><code>find / -perm -2 -type f 2&gt;/dev/null</code></td>
         <td>Find world-writeable files</td>
      </tr>
      <tr>
         <td><code>find / ! -path "*/proc/*" -perm -2 -type f -print 2&gt;/dev/null</code></td>
         <td>Find world-writeable files excluding those in /proc</td>
      </tr>
      <tr>
         <td><code>find / -perm -2 -type d 2&gt;/dev/null</code></td>
         <td>Find word-writeable directories </td>
      </tr>
      <tr>
         <td><code>find /home –name *.rhosts -print 2&gt;/dev/null</code></td>
         <td>Find rhost config files</td>
      </tr>
      <tr>
         <td><code>find /home -iname *.plan -exec ls -la {} ; -exec cat {} 2&gt;/dev/null ;</code></td>
         <td>Find *.plan files, list permissions and cat the file contents</td>
      </tr>
      <tr>
         <td><code>find /etc -iname hosts.equiv -exec ls -la {} 2&gt;/dev/null ; -exec cat {} 2&gt;/dev/null ;</code></td>
         <td>Find hosts.equiv, list permissions and cat the file contents</td>
      </tr>
      <tr>
         <td><code>ls -ahlR /root/</code></td>
         <td>See if you can access other user directories to find interesting files</td>
      </tr>
      <tr>
         <td><code>cat ~/.bash_history</code></td>
         <td>Show the current users’ command history</td>
      </tr>
      <tr>
         <td><code>ls -la ~/.*_history</code></td>
         <td>Show the current users’ various history files</td>
      </tr>
      <tr>
         <td><code>ls -la /root/.*_history</code></td>
         <td>Can we read root’s history files</td>
      </tr>
      <tr>
         <td><code>ls -la ~/.ssh/</code></td>
         <td>Check for interesting ssh files in the current users’ directory</td>
      </tr>
      <tr>
         <td><code>find / -name "id_dsa*" -o -name "id_rsa*" -o -name "known_hosts" -o -name "authorized_hosts" -o -name "authorized_keys" 2&gt;/dev/null |xargs -r ls -la</code></td>
         <td>Find SSH keys/host information</td>
      </tr>
      <tr>
         <td><code>ls -la /usr/sbin/in.*</code></td>
         <td>Check Configuration of inetd services</td>
      </tr>
      <tr>
         <td><code>grep -l -i pass /var/log/*.log 2&gt;/dev/null</code></td>
         <td>Check log files for keywords (‘pass’ in this example) and show positive matches</td>
      </tr>
      <tr>
         <td><code>find /var/log -type f -exec ls -la {} ; 2&gt;/dev/null</code></td>
         <td>List files in specified directory (/var/log)</td>
      </tr>
      <tr>
         <td><code>find /var/log -name *.log -type f -exec ls -la {} ; 2&gt;/dev/null</code></td>
         <td>List .log files in specified directory (/var/log)</td>
      </tr>
      <tr>
         <td><code>find /etc/ -maxdepth 1 -name *.conf -type f -exec ls -la {} ; 2&gt;/dev/null</code></td>
         <td>List .conf files in /etc (recursive 1 level)</td>
      </tr>
      <tr>
         <td><code>ls -la /etc/*.conf</code></td>
         <td>As above</td>
      </tr>
      <tr>
         <td><code>find / -maxdepth 4 -name *.conf -type f -exec grep -Hn password {} ; 2&gt;/dev/null</code></td>
         <td>Find .conf files (recursive 4 levels) and output line number where the word ‘password’ is located</td>
      </tr>
      <tr>
         <td><code>lsof -i -n</code></td>
         <td>List open files (output will depend on account privileges)</td>
      </tr>
      <tr>
         <td><code>head /var/mail/root</code></td>
         <td>Can we read roots mail</td>
      </tr>
   </tbody>
</table>
<p>&nbsp;</p>
<p><b>Service Information:</b></p>
<table width="700px">
   <tbody>
      <tr>
         <th style="width:40%"><b>Command</b></th>
         <th><b>Result</b></th>
      </tr>
      <tr>
         <td><code>ps aux | grep root</code></td>
         <td>View services running as root</td>
      </tr>
      <tr>
         <td><code>ps aux | awk '{print $11}'|xargs -r ls -la 2&gt;/dev/null |awk '!x[$0]++'</code></td>
         <td>Lookup process binary path and permissions</td>
      </tr>
      <tr>
         <td><code>cat /etc/inetd.conf</code></td>
         <td>List services managed by inetd</td>
      </tr>
      <tr>
         <td><code>cat /etc/xinetd.conf</code></td>
         <td>As above for xinetd</td>
      </tr>
      <tr>
         <td><code>cat /etc/xinetd.conf 2&gt;/dev/null | awk '{print $7}' |xargs -r ls -la 2&gt;/dev/null</code></td>
         <td>A very ‘rough’ command to extract associated binaries from xinetd.conf and show permissions of each</td>
      </tr>
      <tr>
         <td><code>ls -la /etc/exports 2&gt;/dev/null; cat /etc/exports 2&gt;/dev/null</code></td>
         <td>Permissions and contents of /etc/exports (NFS)</td>
      </tr>
   </tbody>
</table>
<p>&nbsp;</p>
<p><b>Jobs/Tasks:</b></p>
<table width="700px">
   <tbody>
      <tr>
         <th style="width:40%"><b>Command</b></th>
         <th><b>Result</b></th>
      </tr>
      <tr>
         <td><code>crontab -l -u %username%</code></td>
         <td>Privileged command</td>
      </tr>
      <tr>
         <td><code>ls -la /etc/cron*</code></td>
         <td>Scheduled jobs overview (hourly, daily, monthly etc)</td>
      </tr>
      <tr>
         <td><code>ls -aRl /etc/cron* | awk '$1 ~ /w.$/' 2&gt;/dev/null</code></td>
         <td>What can ‘others’ write in /etc/cron* directories</td>
      </tr>
      <tr>
         <td><code>top</code></td>
         <td>List of current tasks</td>
      </tr>
   </tbody>
</table>
<p>&nbsp;</p>
<p><b>Networking, Routing &amp; Communications:</b></p>
<table width="700px">
   <tbody>
      <tr>
         <th style="width:40%"><b>Command</b></th>
         <th><b>Result</b></th>
      </tr>
      <tr>
         <td><code>/sbin/ifconfig -a</code></td>
         <td>List all network interfaces</td>
      </tr>
      <tr>
         <td><code>cat /etc/network/interfaces</code></td>
         <td>As above</td>
      </tr>
      <tr>
         <td><code>arp -a</code></td>
         <td>Display ARP communications</td>
      </tr>
      <tr>
         <td><code>route</code></td>
         <td>Display route information</td>
      </tr>
      <tr>
         <td><code>cat /etc/resolv.conf</code></td>
         <td>Show configured DNS sever addresses</td>
      </tr>
      <tr>
         <td><code>netstat -antp</code></td>
         <td>Privileged command)</td>
      </tr>
      <tr>
         <td><code>netstat -anup</code></td>
         <td>Privileged command)</td>
      </tr>
      <tr>
         <td><code>iptables -L</code></td>
         <td>Privileged command</td>
      </tr>
      <tr>
         <td><code>cat /etc/services</code></td>
         <td>View port numbers/services mappings</td>
      </tr>
   </tbody>
</table>
<p>&nbsp;</p>
<p><b>Programs Installed:</b></p>
<table width="700px">
   <tbody>
      <tr>
         <th style="width:40%"><b>Command</b></th>
         <th><b>Result</b></th>
      </tr>
      <tr>
         <td><code>dpkg -l</code></td>
         <td>Installed packages (Debian)</td>
      </tr>
      <tr>
         <td><code>rpm -qa</code></td>
         <td>Installed packages (Red Hat)</td>
      </tr>
      <tr>
         <td><code>sudo -V</code></td>
         <td>Sudo version – does an exploit exist?</td>
      </tr>
      <tr>
         <td><code>httpd -v</code></td>
         <td>Apache version</td>
      </tr>
      <tr>
         <td><code>apache2 -v</code></td>
         <td>As above</td>
      </tr>
      <tr>
         <td><code>apache2ctl (or apachectl) -M</code></td>
         <td>List loaded Apache modules</td>
      </tr>
      <tr>
         <td><code>mysql --version</code></td>
         <td>Installed MYSQL version details</td>
      </tr>
      <tr>
         <td><code>psql -V</code></td>
         <td>Installed Postgres version details</td>
      </tr>
      <tr>
         <td><code>perl -v</code></td>
         <td>Installed Perl version details</td>
      </tr>
      <tr>
         <td><code>java -version</code></td>
         <td>Installed Java version details</td>
      </tr>
      <tr>
         <td><code>python --version</code></td>
         <td>Installed Python version details</td>
      </tr>
      <tr>
         <td><code>ruby -v</code></td>
         <td>Installed Ruby version details</td>
      </tr>
      <tr>
         <td><code>find / -name %program_name% 2&gt;/dev/null</code>&nbsp;(i.e. nc, netcat, wget, nmap etc)</td>
         <td>Locate ‘useful’ programs (netcat, wget etc)</td>
      </tr>
      <tr>
         <td><code>which %program_name%</code> (i.e. nc, netcat, wget, nmap etc)</td>
         <td>As above</td>
      </tr>
      <tr>
         <td><code>dpkg --list 2&gt;/dev/null| grep compiler |grep -v decompiler 2&gt;/dev/null &amp;&amp; yum list installed 'gcc*' 2&gt;/dev/null| grep gcc 2&gt;/dev/null</code></td>
         <td>List available compilers</td>
      </tr>
      <tr>
         <td>
            <p></p>
         </td>
         <td>Which account is Apache running as</td>
      </tr>
   </tbody>
</table>
<p>&nbsp;</p>
<p><b>Common Shell Escape Sequences:</b></p>
<table width="700px">
   <tbody>
      <tr>
         <th style="width:40%"><b>Command</b></th>
         <th><b>Program(s)</b></th>
      </tr>
      <tr>
         <td><code>:!bash</code></td>
         <td>vi, vim</td>
      </tr>
      <tr>
         <td><code>:shell</code></td>
         <td>vi, vim</td>
      </tr>
      <tr>
         <td><code>!bash</code></td>
         <td>less</td>
      </tr>
      <tr>
         <td><code>find / -exec /usr/bin/awk 'BEGIN {system("/bin/bash")}' ; </code></td>
         <td>find</td>
      </tr>
      <tr>
         <td><code>awk 'BEGIN {system("/bin/bash")}'</code></td>
         <td>awk</td>
      </tr>
      <tr>
         <td><code>--interactive</code></td>
         <td>nmap</td>
      </tr>
      <tr>
         <td><code>perl -e 'exec "/bin/bash";'</code></td>
         <td>Perl</td>
      </tr>
   </tbody>
</table>
