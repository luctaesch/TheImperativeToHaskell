yes.

 Lets introduce three techniques to have a minimalist reading : 

- layout

- removing parentheses and $ 

- pattern matching and guards.

curly braces, semicolon and parentheses are optional, unless ambiguity need to be raised. 

curly braces are used to delimitate a block. layout can be used instead.

myaction  = do {

			   print "hello"; 

			   print "world/n";

			}

myaction  = do 

			   print "hello"

			   print "world/n"

this would not compile: 

myaction  = do 

			   print "hello"

		print "world/n"

beware : tabulation does not work. they count as one character. have your text editor substitute  spaces instead			

next thing is parentheses.

parentheses can quickly accumulate and become a pain to read. they are optional:

f ( g ( h (x))) = f g h x

..unless they are not :

print map f [1..3] will break the compile ("The function `print' is applied to three argument..")  . Use instead :

print ( map f [1..3] )

or better 

print $ map f [1..3]

 

$ avoid putting parenthesis at the end, which is convenient.

"Anything appearing after it will take precedence over anything that comes before"

print ( uppercase ( "aa" ++ "bb")) = 

print $ uppercase ( "aa" ++ "bb") = 

print $ uppercase $ "aa" ++ "bb"