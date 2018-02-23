# Name
The Password Manager

# Value
300 

# Description

Here's a password manager vault. We picked this up through a compromised dropbox account. They should have enabled 2-FA.

# Hints
-----------------------------------------------------------------

## Hint 1
Here's a really awesome python library for working with the opvault format:
https://github.com/OblivionCloudControl/opvault

## Hint 2
You should not be brute forcing this. Use a common password dictionary.

# Flag

`flag{Wow_You_CRACKED-the-VAULT}`

# Solution

```
tar -xvf neverlan.tar.gz
pip install opvault
opvault-cli neverlan.opvault flag
Password: starwars
```
