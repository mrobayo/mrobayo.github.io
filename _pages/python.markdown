Implement the missing code, denoted by ellipses. You may not modify the pre-existing code.
Given a word, check whether it is a palindrome or not. A string is considered to be a palindrome if it reads the same in both directions.

Example

For word = "aibohphobia", the output should be
isWordPalindrome(word) = true;

For word = "hehehehehe", the output should be
isWordPalindrome(word) = false.

def isWordPalindrome(word):
    return word == word[::-1]


For password = "iamthebest" and
key = "zabcdefghijklmnopqrstuvwxy", the output should be
permutationCipher(password, key) = "hzlsgdadrs".

Here's a table that can be used to encrypt the text:

abcdefghijklmnopqrstuvwxyz
||  |  ||   |     || 
vv  v  vv   v     vv
zabcdefghijklmnopqrstuvwxy
def permutationCipher(password, key):
    table = string.maketrans("abcdefghijklmnopqrstuvwxyz", key)
    return str(password).translate(table)



For t = 3.1415, width = 10, and precision = 2,
the output should be

competitiveEating(t, width, precision) = "   3.14   "

def competitiveEating(t, width, precision):
    return (("{0:."+str(precision)+"f}").format(t)).center(width, ' ')
