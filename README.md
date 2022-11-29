<u>my spotify interface</u>

pulls each word from an insult from the elizabethan insult api to build a playlist comprising of those same words

the intended output would be a spotify playlist whereby the songs can be read as an acrostic for the insult



you will need:

the elizabethan api (no key needed)

https://quandyfactory.com/insult

JSON link:

https://quandyfactory.com/insult/json



for the spotify keys, i used this format:

```
{
'username': 'spotify username',
 'client_id': '...',
 'client_secret': '...',
 'redirect': 'https://www.google.com/'
 }
```

news key is in separate txt doc on its own

*please find versions in requirements.txt



this works although due to the nature of some of the obscure/outdated words within the *elizabethan insult* api, the playlist does not read as fluently as I had hoped

my code has been programmed to search each word of the generated insult for the name of each song but sometimes it will substitute for songs with additional words/words which only contain a fragment of my words, (for instance: no song entitled 'thou' means that it has returned a song called 'a thousand miles' as a substitute which of course negates the purpose of the concept)

redoing this in the future, it would be more productive to work with an api which uses outputs (or insults) with more everyday language as it is more likely that the corresponding song titles could be allocated in order for the playlist to read

with a few substitutions and adaptations, my code could be used for this