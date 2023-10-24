# Competitive-Programming
Given a string s consisting of words and spaces, return the length of the last word in the string. A word is a maximal substring consisting of non-space characters only.
def lengthOfLastWord(s):
    # Split the string by spaces and remove empty strings
    words = s.split()
    
    # Check if there are words in the list
    if words:
        # Get the last word and return its length
        return len(words[-1])
    else:
        # If there are no words, return 0
        return 0

s1 = "Hello World"
print(lengthOfLastWord(s1))  # Output: 5

s2 = "   fly me   to   the moon  "
print(lengthOfLastWord(s2))  # Output: 4
