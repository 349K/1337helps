# wifite command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


[32m  .;'                     `;,    
[32m .;'  ,;'             `;,  `;,   [0mWiFite v2 (r87)
[32m.;'  ,;'  ,;'     `;,  `;,  `;,  
[32m::   ::   :   [37m( )[32m   :   ::   ::  [37mautomated wireless auditor
[32m':.  ':.  ':. [37m/_\[32m ,:'  ,:'  ,:'  
[32m ':.  ':.    [37m/___\[32m    ,:'  ,:'   [37mdesigned for Linux
[32m  ':.       [37m/_____\[32m      ,:'     
[32m           [37m/       \[32m             
[0m
usage: wifite [-h] [--check CHECK] [--cracked] [--recrack] [--all]
              [-i INTERFACE] [--mac] [--mon-iface MONITOR_INTERFACE]
              [-c CHANNEL] [-e ESSID] [-b BSSID] [--showb] [--nodeauth]
              [--power POWER] [--tx TX] [--quiet] [--wpa] [--wpat WPAT]
              [--wpadt WPADT] [--strip] [--crack] [--dict DIC] [--aircrack]
              [--pyrit] [--tshark] [--cowpatty] [--wep] [--pps PPS]
              [--wept WEPT] [--chopchop] [--arpreplay] [--fragment]
              [--caffelatte] [--p0841] [--hirte] [--nofakeauth]
              [--wepca WEPCA] [--wepsave WEPSAVE] [--wps] [--pixie]
              [--wpst WPST] [--wpsratio WPSRATIO] [--wpsretry WPSRETRY]

optional arguments:
  -h, --help            show this help message and exit

COMMAND:
  --check CHECK         Check capfile [file] for handshakes.
  --cracked             Display previously cracked access points.
  --recrack             Include already cracked networks in targets.

GLOBAL:
  --all                 Attack all targets.
  -i INTERFACE          Wireless interface for capturing.
  --mac                 Anonymize MAC address.
  --mon-iface MONITOR_INTERFACE
                        Interface already in monitor mode.
  -c CHANNEL            Channel to scan for targets.
  -e ESSID              Target a specific access point by ssid (name).
  -b BSSID              Target a specific access point by bssid (mac).
  --showb               Display target BSSIDs after scan.
  --nodeauth            Do not deauthenticate clients while scanning
  --power POWER         Attacks any targets with signal strength > [pow].
  --tx TX               Set adapter TX power level.
  --quiet               Do not print list of APs during scan.

WPA:
  --wpa                 Only target WPA networks (works with --wps --wep).
  --wpat WPAT           Time to wait for WPA attack to complete (seconds).
  --wpadt WPADT         Time to wait between sending deauth packets (seconds).
  --strip               Strip handshake using tshark or pyrit.
  --crack               Crack WPA handshakes using [dic] wordlist file.
  --dict DIC            Specificy dictionary to use when cracking WPA.
  --aircrack            Verify handshake using aircrack.
  --pyrit               Verify handshake using pyrit.
  --tshark              Verify handshake using tshark.
  --cowpatty            Verify handshake using cowpatty.

WEP:
  --wep                 Only target WEP networks.
  --pps PPS             Set the number of packets per second to inject.
  --wept WEPT           Sec to wait for each attack, 0 implies endless.
  --chopchop            Use chopchop attack.
  --arpreplay           Use arpreplay attack.
  --fragment            Use fragmentation attack.
  --caffelatte          Use caffe-latte attack.
  --p0841               Use P0842 attack.
  --hirte               Use hirte attack.
  --nofakeauth          Stop attack if fake authentication fails.
  --wepca WEPCA         Start cracking when number of IVs surpass [n].
  --wepsave WEPSAVE     Save a copy of .cap files to this directory.

WPS:
  --wps                 Only target WPS networks.
  --pixie               Only use the WPS PixieDust attack
  --wpst WPST           Max wait for new retry before giving up (0: never).
  --wpsratio WPSRATIO   Min ratio of successful PIN attempts/total retries.
  --wpsretry WPSRETRY   Max number of retries for same PIN before giving up.

~~~
