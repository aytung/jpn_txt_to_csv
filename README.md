# jpn_text_to_csv

A Python3 script to convert a txt file to a csv file to import into Anki. Intended to be used with https://dictionary.goo.ne.jp/jn/"


## Usage 

The text file should be named "anki.txt." 
The output file will be named "anki.csv"

**Important: Make certain that different flashcards are separated by at least one extra newline**

Make certain that all sentences are surrounded by "「" on the left and on "」" the right.

Everything else will convert "blocks" of text to single-sided flashcards.

I.E, 

`「憂鬱は暮れない」\n`

will be converted to 

`「憂鬱は暮れない」, \n`

and

`Ressentiment\n`
`(Vieilli) Faible atteinte, faible renouvellement d’un mal qu’on a eu, d’une douleur qu’on a ressentie.\n`
`(Figuré) (Plus courant) Souvenir douloureux qu’on garde des injures et blessures, avec ou sans désir de s’en venger. \n`

Will be converted to

`Ressentiment, (Vieilli) Faible atteinte, faible renouvellement d’un mal qu’on a eu, d’une douleur qu’on a ressentie.\n`
`(Figuré) (Plus courant) Souvenir douloureux qu’on garde des injures et blessures, avec ou sans désir de s’en venger.\n`

Similarly, singular lines will be converted by themselves;

`儘管還有些遙遠 至少能夠佔據你視線\n`

Will be written as:

`儘管還有些遙遠 至少能夠佔據你視線,\n`
