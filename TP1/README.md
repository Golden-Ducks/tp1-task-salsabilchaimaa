line 17
building strings with += inside a loop is discouraged bcz strings are immutable
use a list or just use .isalnum() filter for better performance

line 10
your words_numbr dict is redundant bcz you're mapping "one" to "one"
you can just skip that check if you're not changing the word

line 12
the logic w.isdigit() and w in n will fail for "10." bcz of the punctuation
maybe clean the punctuation first before checking for digits

line 24
btw, if you use .get() you can simplify these nested if/else checks
