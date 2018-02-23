# Name
SHA-1

# Value
200

# Description

We found a password that might be useful, but it's currently hashed. Can you crack the hash?

We _know_ the first character is a digit, but that's it.

# Hints
-----------------------------------------------------------------

## Hint 1
A well done mask will help here a ton. Oh, the hint. The password only contains letters and numbers. No symbols.

## Hint 2
There's only 1 capitol letter and it's the 4th character.

# Flag

`1stOrder`

# Solution
- hashcat -a 3 -m 100 sha1.txt -1 ?l?u?d ?d?1?1?1?1?1?1?1
