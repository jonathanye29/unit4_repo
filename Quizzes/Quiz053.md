# Quiz 53

<img width="989" alt="Screen Shot 2023-06-19 at 11 08 25 PM" src="https://github.com/jonathanye29/unit4_repo/assets/111751273/f2700e44-832c-4e5c-8eea-ac112d96dd09">

## Code
```.py
class WordCounter():
    def __init__(self,text):
        self.text = text
        self.word_count = {}
    def count_words(self):
        self.word_count = {}
        for char in self.text:
            if char in ",. ":
                self.text = self.text.replace(char, " ")
        for word in self.text.lower().split():
            if word in self.word_count:
                self.word_count[word] += 1
            else:
                self.word_count[word] = 1
    def get_results(self):
        return self.word_count
```

## Evidence
<img width="822" alt="Screen Shot 2023-06-19 at 11 29 40 PM" src="https://github.com/jonathanye29/unit4_repo/assets/111751273/4ce1f76f-964f-4fe8-beca-3a50786f77f7">
