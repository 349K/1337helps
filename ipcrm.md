# ipcrm command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
 ipcrm [options]
 ipcrm shm|msg|sem <id>...

Remove certain IPC resources.

Options:
 -m, --shmem-id <id>        remove shared memory segment by id
 -M, --shmem-key <key>      remove shared memory segment by key
 -q, --queue-id <id>        remove message queue by id
 -Q, --queue-key <key>      remove message queue by key
 -s, --semaphore-id <id>    remove semaphore by id
 -S, --semaphore-key <key>  remove semaphore by key
 -a, --all[=shm|msg|sem]    remove all (in the specified category)
 -v, --verbose              explain what is being done

 -h, --help     display this help and exit
 -V, --version  output version information and exit

For more details see ipcrm(1).

~~~
