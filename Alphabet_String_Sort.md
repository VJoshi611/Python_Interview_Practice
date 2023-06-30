# Alphabet_String_Sort

###  Write a Python program to sort alphabetically the words form a string provided by the user
def sort_words(string):
    words = string.split()                            # Split the string into a list of words
    sorted_words = sorted(words)                      # Sort the words alphabetically
    sorted_string = ' '.join(sorted_words)            # Join the sorted words into a string
    return sorted_string

input = "how are you"
sorted_string = sort_words(input)
print(sorted_string)
