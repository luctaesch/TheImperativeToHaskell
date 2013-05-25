Yes.

List are the workhorse in Haskell.

[ ] denote a list . (not an Array !)  

a String is just a list of Char : String = [Char]

['a','b','c'] = "abc"

some functions on list : 

: add an element in front of the list

'a':"bc" = "abc" = ['a','b','c'] = 'a':'b':'c'

++ joins two list together (concatenate)

"ab"++"cd" = "abcd"

head ("abc") = 'a' 

head gets the head of the list

tail ("abc") = "bc"

head gets the tail of the list, (i.e. the list minus the head)

"abcde"!!2 = 'c' 

!! get the nth item of a list, starting at 0

map (even [1,2,3] )= [False,True,False]

map (f alist) = apply the function f on all the element of list alist

[] is the empty list

- List needs no sizing nor allocation, nor deallocation.

- we will look more at list later (tbd)