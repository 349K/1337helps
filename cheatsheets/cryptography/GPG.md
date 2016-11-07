# **GNU Privacy Guard** CheatSheet
GNU Privacy Guard (GnuPG or GPG) is a free software replacement for Symantec's PGP cryptographic software suite.[6] GnuPG is compliant with RFC 4880, which is the IETF standards track specification of OpenPGP. Modern versions of PGP and Veridis' Filecrypt are interoperable with GnuPG and other OpenPGP-compliant systems.

```GnuPG is part of the GNU project, and has received major funding from the German government.```

------------------------------------------------------------------------------------------------

#### + Table of Contents
##### Create & Export
+ [ Create a key-pair](1-how-to-create-a-key-pair--)
+ [ Export a public key](#2-how-to-export-a-public-key--)
+ [ Export a private key ](#3-how-to-export-a-private-key--)

##### Import Keys
+ [Import a public key](#4-how-to-import-a-public-key-)
+ [Import a private key?](#5-how-to-import-a-private-key--)

##### Delete Keys
+ [Delete a public key?](#6-how-to-delete-a-public-key-from-your-public-key-ring--)
+ [Delete an private key?](#7-how-to-delete-an-private-key-a-key-on-your-private-key-ring---)

##### List Keys
+ [List the keys in your public key ring](#8-how-to-list-the-keys-in-your-public-key-ring--)
+ [list the keys in your private key ring](#9-how-to-list-the-keys-in-your-secret-key-ring--)

##### Usage
+ [Public key verification](#10-how-to-generate-a-short-list-of-numbers-that-you-can-use-via-an-alternative-method-to-verify-a-public-key--)
+ [Encryption](#11-how-to-encrypt-data--)
+ [Decryption](#12-how-to-decrypt-data--)


------------------------------------------------------------------------------------------------

#### 1. How to create a key-pair? [ ](#1)
~~~
gpg --gen-key
~~~
##### Output Screen:
~~~
gpg (GnuPG) 1.4.20; Copyright (C) 2015 Free Software Foundation, Inc.
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

Please select what kind of key you want:
   (1) RSA and RSA (default)
   (2) DSA and Elgamal
   (3) DSA (sign only)
   (4) RSA (sign only)
Your selection? 1
RSA keys may be between 1024 and 4096 bits long.
What keysize do you want? (2048) 4096
Requested keysize is 4096 bits
Please specify how long the key should be valid.
         0 = key does not expire
      <n>  = key expires in n days
      <n>w = key expires in n weeks
      <n>m = key expires in n months
      <n>y = key expires in n years
Key is valid for? (0) 180
Key expires at Fri May  5 14:18:49 2017 EDT
Is this correct? (y/N) y

You need a user ID to identify your key; the software constructs the user ID
from the Real Name, Comment and Email Address in this form:
    "Heinrich Heine (Der Dichter) <heinrichh@duesseldorf.de>"

Real name: John Doe
Email address: john.doe@away.far
Comment: Who am I anyways?
You selected this USER-ID:
    "John Doe (Who am I anyways?) <john.doe@away.far>"

Change (N)ame, (C)omment, (E)mail or (O)kay/(Q)uit? O
You need a Passphrase to protect your secret key.

We need to generate a lot of random bytes. It is a good idea to perform
some other action (type on the keyboard, move the mouse, utilize the
disks) during the prime generation; this gives the random number
generator a better chance to gain enough entropy.
.............................................................+++++
.......+++++
We need to generate a lot of random bytes. It is a good idea to perform
some other action (type on the keyboard, move the mouse, utilize the
disks) during the prime generation; this gives the random number
generator a better chance to gain enough entropy.
....+++++
...+++++
gpg: key 1CD3E2CB marked as ultimately trusted
public and secret key created and signed.

gpg: checking the trustdb
gpg: 3 marginal(s) needed, 1 complete(s) needed, PGP trust model
gpg: depth: 0  valid:   2  signed:   0  trust: 0-, 0q, 0n, 0m, 0f, 2u
gpg: next trustdb check due at 2017-05-05
pub   4096R/1CD3E2CB 2016-11-06 [expires: 2017-05-05]
      Key fingerprint = 3F21 C199 3F21 38D6 D13C  FFA6 346D 7EA8 1CD3 E2CB
uid                  John Doe (Who am I anyways?) <john.doe@away.far>
sub   4096R/DBB6F429 2016-11-06 [expires: 2017-05-05]

~~~



#### 2. How to export a public key? [ ](#2)
~~~
gpg --export -a "John Doe"
~~~
This will create a key called public.key with the ascii representation of the public key for John Doe.
##### Output Screen:
~~~
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: GnuPG v1

mQINBFgfdFoBEACu/rcUWMGLZwyUBIDvX1LqGPUARW5ahgPfg6bZFZ9Sl0+MreOO
y7RzNFjkstMvVvPGoHTdTacsvX/PBPYntVGKp4LYYWqSAjSX6C7ZFouwi0x+dcRX
969ZnovO3x4JHb9wraZccqRhV8pIsvR/+TRMnykHpnrXe4Zq62bLQNIFJeph68qM
...
FzV4YaG0e08168RsIp0rSirjInsX8KaSukxsL4i8gnFI8f8gTM4GZ78LVT6T4a4F
Kb98Ov5a3EqMCuPDqWiWY3XrFqLeGRAhADbh6KrZoeOOt5+HXfaC2aQWnpufT6ro
gUewTp80P3XAkXziYL0i0P/jAkozzajFN05rfVBGtICX1RGKci8h0jBjkC80m1Jv
T5exsyXcP47gSIuKslfM7ABT5Nmhp4YoiTXu
=yHSg
-----END PGP PUBLIC KEY BLOCK-----
~~~


#### 3. How to export a private key? [ ](#3)
~~~
gpg --export-secret-key -a "John Doe"
~~~
This will create a key called private.key with the ascii representation of the private key for John Doe.
It's pretty much like exporting a public key, but you have to override some default protections.

##### Output Screen:
~~~
-----BEGIN PGP PRIVATE KEY BLOCK-----
Version: GnuPG v1

lQdGBFgfdFoBEACu/rcUWMGLZwyUBIDvX1LqGPUARW5ahgPfg6bZFZ9Sl0+MreOO
y7RzNFjkstMvVvPGoHTdTacsvX/PBPYntVGKp4LYYWqSAjSX6C7ZFouwi0x+dcRX
969ZnovO3x4JHb9wraZccqRhV8pIsvR/+TRMnykHpnrXe4Zq62bLQNIFJeph68qM
...
lmN16xai3hkQIQA24eiq2aHjjrefh132gtmkFp6bn0+q6IFHsE6fND91wJF84mC9
ItD/4wJKM82oxTdOa31QRrSAl9URinIvIdIwY5AvNJtSb0+XsbMl3D+O4EiLirJX
zOwAU+TZoaeGKIk17g==
=0OYO
-----END PGP PRIVATE KEY BLOCK-----
~~~


#### 4. How to import a public key?[ ](#4)
~~~
gpg --import public.key
~~~
This adds the public key in the file "public.key" to your public key ring.


#### 5. How to import a private key? [ ](#5)
NOTE: I've been informed that the manpage indicates that "this is an obsolete option and is not used anywhere." So this may no longer work.
~~~
gpg --allow-secret-key-import --import private.key
~~~
This adds the private key in the file "private.key" to your private key ring. There's a note (*) at the bottom explaining why you may want to do this.


#### 6. How to delete a public key (from your public key ring)? [ ](#6)
~~~
gpg --delete-key "User Name"
~~~
This removes the public key from your public key ring.
NOTE! If there is a private key on your private key ring associated with this public key, you will get an error! You must delete your private key for this key pair from your private key ring first.


#### 7. How to delete an private key (a key on your private key ring)?  [ ](#7)
~~~
gpg --delete-secret-key "User Name"
~~~
This deletes the secret key from your secret key ring.


#### 8. How to list the keys in your public key ring? [ ](#8)
~~~
gpg --list-keys
~~~

#### 9. How to list the keys in your secret key ring? [ ](#9)
~~~
gpg --list-secret-keys
~~~


#### 10. How to generate a short list of numbers that you can use via an alternative method to verify a public key? [ ](#10)
~~~
gpg --fingerprint > fingerprint
~~~
This creates the file fingerprint with your fingerprint info.


#### 11. How to encrypt data? [ ](#11)
~~~
gpg -e -u "Sender User Name" -r "Receiver User Name" somefile
~~~
here are some useful options here, such as -u to specify the secret key to be used, and -r to specify the public key of the recipient.
As an example: gpg -e -u "Charles Lockhart" -r "A Friend" mydata.tar

This should create a file called "mydata.tar.gpg" that contains the encrypted data. I think you specify the senders username so that the recipient can verify that the contents are from that person (using the fingerprint?).
NOTE!: mydata.tar is not removed, you end up with two files, so if you want to have only the encrypted file in existance, you probably have to delete mydata.tar yourself.
An interesting side note, I encrypted the preemptive kernel patch, a file of 55,247 bytes, and ended up with an encrypted file of 15,276 bytes.


#### 12. How to decrypt data? [ ](#12)
~~~
gpg -d mydata.tar.gpg
~~~
If you have multiple secret keys, it'll choose the correct one, or output an error if the correct one doesn't exist. You'll be prompted to enter your passphrase. Afterwards there will exist the file "mydata.tar", and the encrypted "original," mydata.tar.gpg.

```NOTE: when I originally wrote this cheat sheet, that's how it worked on my system, however it looks now like "gpg -d mydata.tar.gpg" dumps the file contents to standard output. The working alternative (worked on my system, anyway) would be to use "gpg -o outputfile -d encryptedfile.gpg", or using mydata.tar.gpg as an example, I'd run "gpg -o mydata.tar -d mydata.tar.gpg". Alternatively you could run something like "gpg -d mydata.tar.gpg > mydata.tar" and just push the output into a file. Seemed to work either way.```

Ok, so what if you're a paranoid bastard and want to encrypt some of your own files, so nobody can break into your computer and get them? Simply encrypt them using yourself as the recipient.
I haven't used the commands:
gpg --edit-key
gpg --gen-revoke
--gen-revoke creates a revocation certificate, which when distributed to people and keyservers tells them that your key is no longer valid, see http://www.gnupg.org/gph/en/manual/r721.html
--edit-key allows you do do an assortment of key tasks, see http://www.gnupg.org/gph/en/manual/r899.html
