# CaesarCipher
A basic implementation of the Caesar Cipher encryption using Java.

Caesar Cipher is a simple encryption algorithm. Given a string of letters and a number key (say 'k'), it shifts all the letters of the string by 'k' positions according to the alphabet. If we start with A = 0 we would then have Z = 25. If we consider the letter 'D' and the key as 3 (k = 3), then the letter will be now represented as 'G' which is three places next to D in the alphabet. After Z, we come back to A i.e., it is a cyclic consideration.

(Using the edu.duke library and originally executed in BlueJ environment -- credits to Duke University and Coursera)

Methods used in this project:

CAESAR CIPHER (to perform the encryption):
1) String encrypt(String input, int key) -- the "input" string is encrypted with 'key'. We are encrypting the whole message using only one key.
2) void test() -- to test encrypt()
3) String encryptTwoKeys(String input, int key1, int key2) -- in the "input" string, all the odd positions are encrypted with 'key1', even positions are encrypted with 'key2'
4) void testEcryptTwoKeys() -- to test encryptTwoKeys()

CAESAR BREAKER (Decrypting Caesar Cipher encryption):
1) countLetters() - counts the number of occurences of each letter and stores it in an array
2) maxIndex() - finds out the most-occured letter
3) decrypt() - decrypts the encrypted message (only one key)
4) halfOfString() - returns a new String that is every other character from message starting with the start position
5) getKey() - calls countLetters() and maxIndex() and returns the max freq letter

CAESAR CIPHER II (For the Object-oriented implementation):
1) Construction performs shifting of alphabet using 2-key encryption
2) String encrypt(String input) -- the "input" string is encrypted (2 keys)
3) String decrypt(String input) -- the "input" string is decrypted (2 keys)
4) void simpletests() -- to test the encryption and decryption methods
