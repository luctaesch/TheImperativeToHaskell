Yes.

in C : 

int f(int x, int y) {

    return x*x + y*y;

}

in Haskell : 

f x y = x*x + y*y

However, 

there are two categories:  functions and actions.

f x = ((g (x ))*(h (x) ))/ 2

we do not care if the compiler evaluates g or h first, as long it comes with a good result. this is a function. a function always gives the same result (given the same parameters).

now consider getChar that reads a character from StdIn.

it will NOT give the same result at every call, as it depends on what is comes in from StdIn. this is an action. Note that the sequence matters for actions,  like opening a file first, (do something with it), then close the file. we do care about the sequence for actions.

the syntax to specify the sequence is do {actions1; actions2..}

  copyCharUnlessNL  =  do { c <- getChar ; 

			    if ( c=='/n')

  			       then { putChar ''}			       else { putChar c}

		        } 

// copy a char from stdio to stdout, unless is is a NewLine

The keyword do introduces a sequence of statements which are executed in order. A statement is either an action, or the assignment  of the result of an action using <-. 				

we will come back to this distinction, as this is central to haskell and is a point where many could fails 