(demonstration of map and fold on recursion):

BOB: the previous statement that one cannot mutate variable puzzled me! I cannot imagine working without ..

for instance, in a loop to calculate 

the length of a String:

in C: 

int calculate_length(char *string) {

    int length = 0;

    while (string[length] != '\0') {

        length++;

    }

    return length;

}

trying to do something similar in haskell would be:

mylength s = do  { let l =0

			            for (s)

			                                   			             l = l+1

			        return ( l)

			        }

because as mentioned, one cannot  mutate a variable, and l is mutated in l=l+1 

Simon : 

well, we could use recursion instead of loops:

mylength counter s = 

      if (s==[]) 

      then counter 

      else  mylength (1 + counter) (tail(s)) 

main = print (  mylength 0 "how long?" )

	

mylength is recursing by removing one character ( the head) at a time, and adding one to a counter, until the string is empty, in which case it terminates and results the counter.

 "abc" 0

"bc" 1

"c" 2	

"" 3

this technique is very common. it is called a fold,  and do a computation that "accumulate" a state (the length) when traverse a structure ( the list).

( Cross domain example: a SQL count (or sum) traverse a table and accumulate a count (or sum) )

Note we did not needed to mutate the counter to accumulate its value. we passed it by parameter to the next call.

( questions about performance ? we will see in (tbd))