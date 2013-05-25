Yes 

Pattern Matching work not  only for numerical , lets try on lists :

Lets try an example of a loop.

we iterate over ['a','b',c'] to uppercase each letter.

1/ with brackets and curly braces:

toUppercase (  l ) = { if ( l ==[]) 

                         then  [] 

                         else { uppercase (head(l ): toUppercase (tail (l))}

}

2/lets remove the brackets and curly braces

toUppercase   l  =  if ( l ==[]) 

                         then  [] 

                         else  uppercase $ head l : toUppercase $ tail l

3/lets use pattern matching

toUppercase   []  =  []

toUppercase x:xs =  uppercase x : toUppercase xs

x:xs matches the head and the tail of a list. names are free, you can choose to name it y:z, or peer:apple, what matters is the matching to the : operator, which makes it matches to head and tail of a list.

aList = head(aList):tail(aList)

BOB: this looks neat, so is it how I do most of my loops ?

Simon: well, Indeed, and however I got a trick for you…