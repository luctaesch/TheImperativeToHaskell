Bob : Can I generalize this loop stuff ?

Simon : look at map

map f  []               =  [] map f (x:xs)            =  f x : map f xs

map uppercase ['a','b',c'] = 

uppercase a : map uppercase [ 'b', ' c']= 

'A' : uppercase 'b' : map uppercase 'c' = 'A':'B': uppercase 'c': map uppercase []

= 'A':'B':'C':[] = "ABC"

so we could use map to define the previous function toUppercase

toUppercase l = map uppercase l

Bob: wow, this is going to be hard to do more terse…

Simon : indeed

map is doing all the recursion loop stuff for us. note that we are passing a function as as argument (uppercase). this is possible in haskell.

map is one of the workhorse in haskell, the 'for' loop of haskell when you need to do something with each element of a list. if you need to carry something across, like when you count , or sum, you use fold, the other workhorse.

fold f accu [] = accu

fold f accu x:xs = f x ( fold f accu xs) 

Let s try to sum a list, with (+) a b = a + b .  

( parentheses needed when to use the + function as prefix ) .

fold (+)  0 [1,2,3] =  fold (+) ( (+) 0 1) 	 [2,3]

= fold (+) 1 [2,3] = fold (+) ((+) 1  2) [3] = fold (+) (3) [3] 

= fold ((+) 3 3) [] = fold 6 [] = 6