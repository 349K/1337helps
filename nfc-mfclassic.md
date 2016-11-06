# nfc-mfclassic command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: nfc-mfclassic f|r|R|w|W a|b <dump.mfd> [<keys.mfd> [f]]
  f|r|R|w|W     - Perform format (f) or read from (r) or unlocked read from (R) or write to (w) or unlocked write to (W) card
                  *** format will reset all keys to FFFFFFFFFFFF and all data to 00 and all ACLs to default
                  *** unlocked read does not require authentication and will reveal A and B keys
                  *** note that unlocked write will attempt to overwrite block 0 including UID
                  *** unlocking only works with special Mifare 1K cards (Chinese clones)
  a|A|b|B       - Use A or B keys for action; Halt on errors (a|b) or tolerate errors (A|B)
  <dump.mfd>    - MiFare Dump (MFD) used to write (card to MFD) or (MFD to card)
  <keys.mfd>    - MiFare Dump (MFD) that contain the keys (optional)
  f             - Force using the keyfile even if UID does not match (optional)
Examples: 

  Read card to file, using key A:

    nfc-mfclassic r a mycard.mfd

  Write file to blank card, using key A:

    nfc-mfclassic w a mycard.mfd

  Write new data and/or keys to previously written card, using key A:

    nfc-mfclassic w a newdata.mfd mycard.mfd

  Format/wipe card (note two passes required to ensure writes for all ACL cases):

    nfc-mfclassic f A dummy.mfd keyfile.mfd f
    nfc-mfclassic f B dummy.mfd keyfile.mfd f


~~~
