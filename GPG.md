# **GNU Privacy Guard** CheatSheet
GNU Privacy Guard (GnuPG or GPG) is a free software replacement for Symantec's PGP cryptographic software suite.[6] GnuPG is compliant with RFC 4880, which is the IETF standards track specification of OpenPGP. Modern versions of PGP and Veridis' Filecrypt are interoperable with GnuPG and other OpenPGP-compliant systems.

```GnuPG is part of the GNU project, and has received major funding from the German government.```

------------------------------------------------------------------------------------------------

#### + Table of Contents
##### Create & Export
+ [ Create a key-pair](#1)
+ [ Export a public key](#2)
+ [ Export a private key ](#3)

##### Import Keys
+ [Import a public key](#4)
+ [Import a private key?](#5)
 
##### Delete Keys
+ [Delete a public key?](#6)
+ [Delete an private key?](#7) 

##### List Keys
+ [List the keys in your public key ring](#8)
+ [list the keys in your private key ring](#9)

##### Usage
+ [Public key verification](#10)
+ [Encryption](#11)
+ [Decryption](#12)
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
wX3TDhNIBEWuNJ+D0geEg+wgrtpE1cTHZrDgN9Ju1YCvdSW2nEsli32i9dzuo++v
nYfG9X7ufedGgtDnnltO6VxOUwPLjgfIEqXuhU4xCGubWaM97HOzR68DSjXsq6s+
svrIpS+r0SOEJjJLXwAqitOS2vl+7HfE00WLR/4GsBNjf3hFYFraeunfeDPsPd7o
PsGY6r568tvQrsB1W5fB5M3Kralt36kP5/76FOjWBGPjTkSWKNnY2mZJfeZV1uP9
eyP83AEcZMcj3Zw8MrbAmwujNPchunkIg/jK3B9Fq1sSStmM01bFdIJWBdiDM1pE
rCX7XNCow6qEE8AyHiXBxEWiyQknr8zMcvcW6Mi8bOshPaqpWdCrpaUDqe06Ci6o
PU+efkdwFM079fMoVNHYtH1boz6o4YNxWQzuuCyB9VFzq1fG30E6UgsOuRwVmdZV
CsbZe5G63yQymeNf8NOMOG0o5Y7J0RZ7l0OHjEGkLIW2YuIcc2NzJbteZwARAQAB
tDBKb2huIERvZSAoV2hvIGFtIEkgYW55d2F5cz8pIDxqb2huLmRvZUBhd2F5LmZh
cj6JAj4EEwECACgFAlgfdFoCGwMFCQDtTgAGCwkIBwMCBhUIAgkKCwQWAgMBAh4B
AheAAAoJEDRtfqgc0+LLiTMQAJjgWXG+SdtLCyoY5UWxioDIgZAbvCnKMTRcP4jy
nZcOP3wB1+WYEr+79hvNVblwAum43FvRPIsjy8TbhmIF7yLribnvbEFudnM7OF/3
7MOWaWwUqwPQYs0sEVW1wFB1ZI0IolyRUQVs15dOnbVHqkMe22QPElRQcuSg7DvS
qIQ87LtV7tVBsKyncQTYSRnrsNMjW+q5Ohfyebv1RO6tRzoDJgrO505dZKg2USF+
gtGogB7X+QUORsXgeRIwIcdIQ9OPoJwEk97L81pr2lDdpM/F7cToWbg23L9M9Dgr
g/DJrfAdF55auq1g+tdFsWRtcewFG/tjGZAXwREJNF4ZHFmXJGWCASEnaiQ9DAVx
PDFoE59O/oKN+yYTkDPgiOyqWddfdRTfO7Hgjeuy5XwqyYo0XyCLUiFXvgsBGzMZ
Kz73WdhKI/jgZxynxZLAMueUJmwD4+XjzysB90KuzGiNeLrnaVeS29JhKcNlTEQv
13mjnVHciJzCLhZ74s+RwGQrugpSVCYLJRFWprIJx5qaVZeVsHTDxbT9ri/sQN6k
gGoIdefssRZQ5J3C93rkhXnE15mLcC7XLxUON32gT4sQXSKZRke3PkePbLcnth+i
ZIvfmkL3YSoe2No3KVtqGG8myucA23PYmIVKbM1uk2zuT+R+JKbYkqbE+aR79r+x
gMIduQINBFgfdFoBEADww6a9GfdEb35jJGM6g/IP5L6phtWOcmkVIrMpRiqNekou
0mF4PQMeDB5wXUq4ZP7gUWG04w5no7XUeJF3ly25qed3DRYn21ORms+N6gpZK5wB
gsRYJZPCBLYoMod7dJ5Ev9KhgxCUVxW1I6BkH8ClYREBTVscZWapc3AlxOivRqoo
+CsVAvnboN3NV7dhPyHF/PgMV5U61LsavfyadgEzST32VYhQQpmBgNFhxKJmBxOH
sp0lZPjRkOUIwRwzlBxT9PXBEaLkGVEDoBdkGfV9D82IeU4qYhckBx/B/sStCmkR
qSIW9CHaujiXVhtf/ZVnkAUeBOKl5KRhhyfrQI/KEx7OpJ//LFp2auJTDRiMIlzm
7cRyLhIUWcn9SgWyZBVceYSfPClOdE6hpVuReIxMpQJRfiawokitvoQGY4YmLLib
aPXWDZvuB7iUjiXnRGJS8GA0h/dVq6TnU8VnWamd1Cva8uZx654RhKAWCQPT0IOC
ZW8FC2ceeT2UCJr7Yp/TSikubYXFnGzPPUeJGBAtqMSa3cgFUnWzS3O7Nl7HohZ/
E5xbsVEzSNORyp9SDMHPnWs9HkZG9iYd5PXc5sXWxZ687OxsGp4hWj2Kn4r6CmNk
f295HfNO8DANEr6NP2ep+s4EhGH+ikRVNaUR6J3b0re2xbKUQX5qcdzd3yztVwAR
AQABiQIlBBgBAgAPBQJYH3RaAhsMBQkA7U4AAAoJEDRtfqgc0+LLGjUP/1pswzYV
ZNJQDv2BVQ1lZGfiPMG/EgF+4g/+eEuvxBbDv971dICfKrhgO7z+47oyPmn4E36o
nVAY0N7kinHxa8TB/FcctOalhd1kDQCfv6rxytZ3ZH9adDlMejyCPJvLfs8VXSGm
Fk/aWh/lrO4trHivCMyc1tSDelssrrwrGdSpnrY/+46UnKCDd2kvXzReGLpk61JI
oVNzUGHnwnBSFqZNXuuD6HwmeLxeo2JHZH6wthkH2an9LUBmAXKF2FGR/9Qemof0
h0drJhh6vr9KYIk95L+CZGwnRlUGrIrrTcxl2+VVG2ZL80aECk0eDUY/9n3M/1dP
wUDUhpa5t6wARf3k+68nCj+y6bRkPFxtfBtuDORRxCb7Oxh2oclUIGXjh7cKc7Sw
Tv+SsMnDIpMKEtKJ9U8+2tZSnspjP/vpjnGKShgJ17EF+BIuvvXqsAxLkKsyOb65
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

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
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

