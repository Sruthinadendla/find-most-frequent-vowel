# find-most-frequent-vowel
from collections import Counter
def FindMostFrequentVowel(words):
  vowels=set("aeiouAEIOU")
  x1=Counter(c for c in words if c in vowels)
  Keymax=max(x1,key=lambda x:x1[x])
  return(Keymax)
words=input()
print(FindMostFrequentVowel(words))
