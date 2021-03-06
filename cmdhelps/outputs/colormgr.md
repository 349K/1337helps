# colormgr command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
  colormgr [OPTION...]

  create-device [ID] [SCOPE] [KIND]
                                    Create a device
  create-profile [ID] [SCOPE]       Create a profile
  delete-device [ID|PATH]           Deletes a device
  delete-profile [ID|PATH]          Deletes a profile
  device-add-profile [ID|PATH] [ID|PATH]
                                    Add a profile to a device that already exists
  device-get-default-profile [ID|PATH]
                                    Gets the default profile for a device
  device-get-profile-for-qualifier [ID|PATH] [QUALIFIER]
                                    Returns all the profiles that match a qualifier
  device-inhibit [ID|PATH] [TIMEOUT|0]
                                    Inhibits color profiles for this device
  device-make-profile-default [ID|PATH] [ID|PATH]
                                    Makes a profile default for a device
  device-set-enabled [ID|PATH] [TRUE|FALSE]
                                    Enables or disables the device
  device-set-kind [ID|PATH] [KIND]  Sets the device kind
  device-set-model [ID|PATH] [MODEL]
                                    Sets the device model
  device-set-serial [ID|PATH] [SERIAL]
                                    Sets the device serial
  device-set-vendor [ID|PATH] [VENDOR]
                                    Sets the device vendor
  dump                              Dump all debug data to a file
  find-device [ID]                  Find a device from the device ID
  find-device-by-property [KEY] [VALUE]
                                    Find a device with a given property value
  find-profile [ID]                 Find a profile from the profile ID
  find-profile-by-filename [FILENAME]
                                    Find a profile by filename
  get-devices                       Gets all the color managed devices
  get-devices-by-kind [KIND]        Gets all the color managed devices of a specific kind
  get-profiles                      Gets all the available color profiles
  get-sensor-reading [KIND]         Gets a reading from a sensor
  get-sensors                       Gets all the available color sensors
  get-spectral-reading [KIND]       Gets a spectral reading from a sensor
  get-standard-space [TYPE]         Get a standard colorspace
  import-profile [FILENAME]         Import a profile and install it for the user
  profile-set-property [ID|PATH] [KEY] [VALUE]
                                    Sets extra properties on the profile
  sensor-lock                       Locks the color sensor
  sensor-set-options [KEY] [VALUE]  Sets one or more sensor options

Help Options:
  -h, --help        Show help options

Application Options:
  -v, --verbose     Show extra debugging information
  --version         Show client and daemon versions
  --value-only      Show the value without any header
  --filter          Filter object properties when displaying


~~~
