# Name
Encoding != Hashing

# Value
100 

# Description

Here's a PCAP. Get BashNinja's Password to the Jedi Archives. Profit

# Hints
-----------------------------------------------------------------

## Hint 1
Take a look at all the http traffic

## Hint 2
HTTP Basic Auth. Google it. :)

# Flag

`flag{help-me-obiwan}`

# Solution

- Open in Wireshark.
- Filter to `http` traffic.
- Follow the HTTP traffic until you see `Authorization: Basic YmFzaE5pbmphOmZsYWd7aGVscC1tZS1vYml3YW59`
- Base64 Decode that.
- Submit the flag!
