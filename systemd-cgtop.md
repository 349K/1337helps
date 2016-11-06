# systemd-cgtop command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

systemd-cgtop [OPTIONS...] [CGROUP]

Show top control groups by their resource usage.

  -h --help           Show this help
     --version        Show package version
  -p --order=path     Order by path
  -t --order=tasks    Order by number of tasks/processes
  -c --order=cpu      Order by CPU load (default)
  -m --order=memory   Order by memory load
  -i --order=io       Order by IO load
  -r --raw            Provide raw (not human-readable) numbers
     --cpu=percentage Show CPU usage as percentage (default)
     --cpu=time       Show CPU usage as time
  -P                  Count userspace processes instead of tasks (excl. kernel)
  -k                  Count all processes instead of tasks (incl. kernel)
     --recursive=BOOL Sum up process count recursively
  -d --delay=DELAY    Delay between updates
  -n --iterations=N   Run for N iterations before exiting
  -b --batch          Run in batch mode, accepting no input
     --depth=DEPTH    Maximum traversal depth (default: 3)
  -M --machine=       Show container

~~~
