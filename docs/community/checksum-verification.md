# Checksum and Signature Verification

If you would like to verify the checksum and signature of a download, please perform the following steps:

* Download the package, signature and SHASUMS files
* Verify the SHASUMS matches the package file
* Verify the package file is properly signed

For example:

```bash
# Download the package and signature files.
wget https://spunkybot.de/download/spunkybot-1.14.0.tar.gz
wget https://spunkybot.de/download/spunkybot-1.14.0.tar.gz.asc
wget https://spunkybot.de/download/1.14.0/SHASUMS
wget https://spunkybot.de/download/1.14.0/SHASUMS.sig

# Verify the SHASUMS matches the package file.
shasum -a 256 -c SHASUMS

# Import our public key - one-time step.
$ wget -qO- http://www.alexanderkress.de/pgp_github_key.asc | gpg --import
# Verify the signature files.
$ gpg --verify spunkybot-1.14.0.tar.gz.asc spunkybot-1.14.0.tar.gz
$ gpg --verify SHASUMS.sig SHASUMS
```
