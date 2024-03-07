# word-game
Ram is attempting to create his own text editor with a unique word correction feature. However, the rules for word correction in this editor are quite unusual. Ram believes that if a word contains two consecutive vowels, it's somewhat odd and needs correction. 

n = int(input().strip())
word = input().strip()

corrected_word = ""

for i in range(n):
    if i < n - 1 and (word[i] in "aeiouy") and (word[i + 1] in "aeiouy"):
        continue
    
    corrected_word += word[i]

print(corrected_word)
