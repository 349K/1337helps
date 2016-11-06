# pamon command Help

 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


pamon [options]
Capture audio data from a PulseAudio sound server and write it to STDOUT or the specified file.

  -h, --help                            Show this help
      --version                         Show version

  -r, --record                          Create a connection for recording
  -p, --playback                        Create a connection for playback

  -v, --verbose                         Enable verbose operations

  -s, --server=SERVER                   The name of the server to connect to
  -d, --device=DEVICE                   The name of the sink/source to connect to
  -n, --client-name=NAME                How to call this client on the server
      --stream-name=NAME                How to call this stream on the server
      --volume=VOLUME                   Specify the initial (linear) volume in range 0...65536
      --rate=SAMPLERATE                 The sample rate in Hz (defaults to 44100)
      --format=SAMPLEFORMAT             The sample type, one of s16le, s16be, u8, float32le,
                                        float32be, ulaw, alaw, s32le, s32be, s24le, s24be,
                                        s24-32le, s24-32be (defaults to s16ne)
      --channels=CHANNELS               The number of channels, 1 for mono, 2 for stereo
                                        (defaults to 2)
      --channel-map=CHANNELMAP          Channel map to use instead of the default
      --fix-format                      Take the sample format from the sink/source the stream is
                                        being connected to.
      --fix-rate                        Take the sampling rate from the sink/source the stream is
                                        being connected to.
      --fix-channels                    Take the number of channels and the channel map
                                        from the sink/source the stream is being connected to.
      --no-remix                        Don't upmix or downmix channels.
      --no-remap                        Map channels by index instead of name.
      --latency=BYTES                   Request the specified latency in bytes.
      --process-time=BYTES              Request the specified process time per request in bytes.
      --latency-msec=MSEC               Request the specified latency in msec.
      --process-time-msec=MSEC          Request the specified process time per request in msec.
      --property=PROPERTY=VALUE         Set the specified property to the specified value.
      --raw                             Record/play raw PCM data.
      --passthrough                     Passthrough data.
      --file-format[=FFORMAT]           Record/play formatted PCM data.
      --list-file-formats               List available file formats.
      --monitor-stream=INDEX            Record from the sink input with index INDEX.

~~~
