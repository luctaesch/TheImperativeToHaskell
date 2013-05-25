Yes.

for ("abc" uppercase) = "ABC"

for ([1,2,3] even) = [False, True, False]

for (list function) iterates a function  over the list , and generates a list of results.

However…

the canonical way in Haskell is map.

for is just another way to say map with the arguments flipped.

 

for ("abc" uppercase)  = map ( uppercase "abc") = "ABC"

for (alist f) = map (f alist )