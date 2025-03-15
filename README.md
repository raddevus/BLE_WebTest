## OPENSSL Config File
The openssl .cnf file is required bec browsers need the distinguished name to match the CN (common name) and without the cnf there is no way to make them match.

Here's the sample openssl command: (also included in the `openssl_cmd.sh` command in the repo

`openssl req -x509 -newkey rsa:2048 -keyout NLkey.pem -out NLcert.pem -days 365 -nodes -config openssl.cnf`



