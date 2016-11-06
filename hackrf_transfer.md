# hackrf_transfer command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage:
	[-d serial_number] # Serial number of desired HackRF.
	-r <filename> # Receive data into file (use '-' for stdout).
	-t <filename> # Transmit data from file (use '-' for stdin).
	-w # Receive data into file with WAV header and automatic name.
	   # This is for SDR# compatibility and may not work with other software.
	[-f freq_hz] # Frequency in Hz [0MHz to 7250MHz].
	[-i if_freq_hz] # Intermediate Frequency (IF) in Hz [2150MHz to 2750MHz].
	[-o lo_freq_hz] # Front-end Local Oscillator (LO) frequency in Hz [84MHz to 5400MHz].
	[-m image_reject] # Image rejection filter selection, 0=bypass, 1=low pass, 2=high pass.
	[-a amp_enable] # RX/TX RF amplifier 1=Enable, 0=Disable.
	[-p antenna_enable] # Antenna port power, 1=Enable, 0=Disable.
	[-l gain_db] # RX LNA (IF) gain, 0-40dB, 8dB steps
	[-g gain_db] # RX VGA (baseband) gain, 0-62dB, 2dB steps
	[-x gain_db] # TX VGA (IF) gain, 0-47dB, 1dB steps
	[-s sample_rate_hz] # Sample rate in Hz (4/8/10/12.5/16/20MHz, default 10MHz).
	[-n num_samples] # Number of samples to transfer (default is unlimited).
	[-c amplitude] # CW signal source mode, amplitude 0-127 (DC value to DAC).
	[-R] # Repeat TX mode (default is off) 
	[-b baseband_filter_bw_hz] # Set baseband filter bandwidth in Hz.
	Possible values: 1.75/2.5/3.5/5/5.5/6/7/8/9/10/12/14/15/20/24/28MHz, default < sample_rate_hz.

~~~
