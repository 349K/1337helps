# rtpmixsound command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


rtpmixsound - Version 3.0
              January 03, 2007
 Usage:
 Mandatory -
	pathname of file whose audio is to be mixed into the
	    targeted live audio stream. If the file extension is
	    .wav, then the file must be a standard Microsoft
	    RIFF formatted WAVE file meeting these constraints:
	      1) header 'chunks' must be in one of two sequences:
	           RIFF, fmt, fact, data
	             or
	           RIFF, fmt, data
	      2) Compression Code = 1 (PCM/Uncompressed)
	      3) Number of Channels = 1 (mono)
	      4) Sample Rate (Hz) = 8000
	      5) Significant Bits/Sample =
	              signed,   linear 16-bit or
	              unsigned, linear  8-bit
	    If the file name does not specify a .wav extension,
	    then the file is presumed to be a tcpdump formatted
	    file with a sequence of, exclusively, G.711 u-law
	    RTP/UDP/IP/ETHERNET messages
	    Note: Yep, the format is referred to as 'tcpdump'
	          even though this file must contain udp messages
 Optional -
	-a source RTP IPv4 addr
	-A source RTP port
	-b destination RTP IPv4 addr
	-B destination RTP port
	-f spoof factor - amount by which to:
	     a) increment the RTP hdr sequence number obtained
	        from the ith legitimate packet to produce the
	        RTP hdr sequence number for the ith spoofed packet
	     b) multiply the RTP payload length and add that
	        product to the RTP hdr timestamp obtained from
	        the ith legitimate packet to produce the RTP hdr
	        timestamp for the ith spoofed packet
	     c) increment the IP hdr ID number obtained from the
	        ith legitimate packet to produce the IP hdr ID
	        number for the ith spoofed packet
	   [ range: +/- 1000, default: 2 ]
	-i interface (e.g. eth0)
	-j jitter factor - the reception of a legitimate RTP
	     packet in the target audio stream enables the output
	     of the next spoofed packet. This factor determines
	     when that spoofed packet is actually transmitted.
	     The factor relates how close to the next legitimate
	     packet you'd actually like the enabled spoofed packet
	     to be transmitted. For example, -j 10 means 10% of
	     the codec's transmission interval. If the transmission
	     interval = 20,000 usec (i.e. G.711), then delay the
	     output of the spoofed RTP packet until the time-of-day
	     is within 2,000 usec (i.e. 10%) of the time the next
	     legitimate RTP packet is expected. In other words,
	     delay 100% minus the jitter factor, or 18,000 usec
	     in this example. The smaller the jitter factor, the
	     greater the risk you run of not outputting the
	     spoofed packet before the next legitimate RTP packet
	     is received. Therefore, a factor >= 10 is advised.
	   [ range: 0 - 80, default: 80 = output spoof ASAP ]
	-p seconds to pause between setup and injection
	-h help - print this usage
	-v verbose output mode

Note: If you are running the tool from a host with multiple
      ethernet interfaces which are up, be forewarned that
      the order those interfaces appear in your route table
      and the networks accessible from those interfaces might
      compel Linux to output spoofed audio packets to an
      interface different than the one stipulated by you on
      command line. This should not affect the tool unless
      those spoofed packets arrive back at the host through
      the interface you have specified on the command line
      (e.g. the interfaces have connectivity through a hub).

~~~
