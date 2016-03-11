# fileFloat
Cross platform secure python cloud sync application to work with amazon S3.

This project aims to solve x problems with current cloud syncing solutions.
1. Lack of control
2. Lack of cross platform compatiblity
3. Cost
4. Security

As an avid user of linux, windows, and android I find that most syncing applications are not up to standards. Dropbox comes the closest, but the linux client is far from perfect.

Most syncing services do not offer very transparent security. I want to know what encryption method was used and what key was used. I also only want to store encrypted files. An unencrypted file should never be stored on the cloud. For this reason, all encryption and decryption must happen on the users machine or phone.

Most syncing applications that offer this sort of fine tuned security are not free. fileFloat will use amazon S3, coming in at $0.03 per GB per month.

#TODO
- [ ] Encryption / Decryption
- [ ] Database to persist sync data. Time stamp, subdirectory, file name and extension type. This is to be encrypted and stored on the S3 server
- [ ] Monitor folder for changes in files and new files. Store information into database
- [ ] Upload / Download files from amazon according to database time information
- [ ] Initialization script to set up a folder for sync
- [ ] Android implementation must be able to encrypt and decrypt on local device

