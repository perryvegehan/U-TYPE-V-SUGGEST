# U-TYPE-V-SUGGEST
A team effort to develop a command line based application written in C to provide certain functionalities on a written English piece. The mentioned functionalities include spelling mistake identification and their rectification based on a suggestion algorithm, finding the word token count and rectifying basic grammatical and syntactical errors.

THE SUGGESTIONS:
This is the most interesting part. We aim to provide 10 suggestions for a given wrong spelled word. The suggestions should be arranged so as the most obvious one should be the first and so on.
Eg:
word- aple
suggestions- apple,  applet, maple, apply........

For this we have a dictionary which contains every possible word in english language( around 6-7 lakhs). this dictionary is used throughout this project.

The basic algorithm is to take the wornged word then find the count of matching letters it has with each word.
Also, if the user has written a 4 letter word, then it is highly likely that he meant a ten lettered word. So, we will apply this method to words which have a length of
len-3 to len+3 where len=length of user's word.
Eg: word=aple. len=4  So the algorithms will suggest the word who have a length between 4-2  to 4+2  (ie.) 2 to 6.
Now afer filtering out these words, find how many characters they have in common with the user's word.
Eg: user_word=aple.
Common letters with apple=4
Common letters with applet=4
Common letters with maple=4 
Common letters with apply=3 and so on.

then just display a list of these words and then another exiting thing.

Wait for user's input now: Fow instance:
1) apple
2) applet
3) maple
4) apply
Now the user will enter a number from 1 to 4. Depending on his input, choose the corresponding word and replace it with the wronged word in the original file. And voila!!


Any suggestions to optimize this algo are highly appreciated.
