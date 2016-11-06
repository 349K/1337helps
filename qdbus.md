# qdbus command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: qdbus [--system | --address ADDRESS] [--literal] [servicename] [path] [method] [args]

  servicename       the service to connect to (e.g., org.freedesktop.DBus)
  path              the path to the object (e.g., /)
  method            the method to call, with or without the interface
  args              arguments to pass to the call
With 0 arguments, qdbus will list the services available on the bus
With just the servicename, qdbus will list the object paths available on the service
With service name and object path, qdbus will list the methods, signals and properties available on the object

Options:
  --system          connect to the system bus
  --address ADDRESS connect to the given bus
  --literal         print replies literally

~~~
