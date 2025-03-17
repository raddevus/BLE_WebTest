## OPENSSL Config File
The openssl .cnf file is required bec browsers need the distinguished name to match the CN (common name) and without the cnf there is no way to make them match.

Here's the sample openssl command: (also included in the `openssl_cmd.sh` command in the repo

`openssl req -x509 -newkey rsa:2048 -keyout NLkey.pem -out NLcert.pem -days 365 -nodes -config openssl.cnf`

## Working On MacOS -- But Not On Linux (Ubuntu 24.04)
I had this working on macOS over weekend, but then I couldn't get it working on my Ubuntu 24.04.

Then I discovered in the MDN docs the following:
![image](https://github.com/user-attachments/assets/75be05cd-fc5b-43d1-a27f-2c8c5af0e185)

#### "Linux support not enabled by default"
That is a very ambiguous statement, bec it sounds like there is a way to enable it manually or something.<br>
But the point seems to mean that MS Edge on Linux does not support Bluetooth. 

### This Project Was Simply About Discovering If BLE Was Supported in Browsers
Ok, that's what this project was all about.<br>
Answer: It's not
