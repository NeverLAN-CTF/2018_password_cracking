# Name
The WIFI Network

# Value
200

# Description

So we're still trying to get into the Jedi Archives. Let's try cracking the WiFi. Here's a WPA2 Handshanke I picked up while near the building.

# Hints
-----------------------------------------------------------------

## Hint 1
Don't bruteforce this. Use a common password dictionary.

## Hint 2
I like to use hashcat but hashcat doesn't read from a `.cap` file. It wants a `.hccapx` file.

Here's some instructions on how to get it loaded into hashcat:
- Use `cap2hccapx` (https://hashcat.net/cap2hccapx/)
- `./cap2hccapx neverlan.cap neverlan.hccapx`
- `hashcat -a 0 -m 2500 neverlan.hccapx wordlist.txt`

# Flag

`obiwan17`

# Solution

- Use `cap2hccapx` (https://hashcat.net/cap2hccapx/)
- `./cap2hccapx neverlan.cap neverlan.hccapx`
- `hashcat -a 0 -m 2500 neverlan.hccapx ~/Downloads/rockyou.txt`
- Wait until it finishes and shows the flag
