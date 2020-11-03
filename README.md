# Rovarsparket

word=str(input("Please insert a word: "))

vowels=["a","e","i","o","u"]

def new_word(word):
  newword = []
  for char in word: 
    if char.isalpha() and char not in vowels:
      newword.append(char+"o"+char)
    else:
      newword.append(char)

  return "".join(newword)

finalword = new_word(word)
print(finalword)
