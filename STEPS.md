# Extracting Technical Skills
***
This task seemed easy to me at first, before I took a glance at the dataset, and then I checked it, I was confused. It took me a while to even start doing it. But I did something, and this is what I was able to come up with.

## Steps
1. I started by checking out the Example dataset. The very first thing that caught my eye was that the dataset only had one *feature*. What made the task even more harder for me was that It only had positive examples. I've never worked with such a dataset, but I continued my exploration.
2. The second thing I did was to try to somehow vectorize the strings, but I thought it was quite pointless (at that moment) because I only had one class and classification by converting to vectors was not possible.
3. The third thing I did and What I chose to keep was to try to extract the Parts of Speech of the entries in the dataset. I found out that most of the skills had the name of an Organization or some entity in them. And since I knew that the dataset only contained positive examples, I added the rest of the entries which didn't have recognizable entity names into a Phrase matcher in Spacy (Spacy was the package I used for NLP)
4. After I did this, I realized that now I had to apply it to the raw skills dataset, But I had to clean it. And on checking that dataset, I realized, the only cleaning it required was the removal of Punctuation marks, so I did exactly that, with the help of spacy.
5. Now, I had a possible method of extraction, But, I had no method of testing how accurate it is, as I haven't faced a challenge like this before. So, I decided to drop the idea of testing it.

The file which has to deal with experimenting with the example dataset is [One](One.ipynb), and the one where I tried to apply it to the raw skills dataset is [Two](Two.ipynb)