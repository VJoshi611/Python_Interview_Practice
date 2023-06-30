# Reverse String without using in-built function

method_1 :

def reverse_string(str):
    rev_str = ""
    for i in range(len(str)-1,-1,-1):
        rev_str = rev_str+str[i]
    print(rev_str)

str="geeks"
reverse_string(str)


method_2 :

def reverse_string1(str):
  rev_str1 = ""
  for i in str:
    rev_str1 = i + rev_str1
  return rev_str1
