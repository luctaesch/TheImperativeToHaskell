Ignorance generates pain and suffering when you start. but especially , ignorance linked to assumptions that are not adequate any more when haskelling.

in most other languages, to get to a running program, is 10% compiler and syntax fight, and 90% debug . In Haskell, this is the opposite.

Most of the time, this is not seen, and it hurts because we have the wrong assumptions.

Knowing this is key not to lose the spirit when starting.

why is that, first ? 

a C compiler has a simple system and when you do things too complex for it  to understand, you cast or revert to pointers. If you are wrong, you will see it at debug time. If you want to divide a boolean by a number , it is up to you.  

in Haskell,  the type systems is much more sophisticated so you can express complex things. There is no such things as a cast. That means no possible cheating when getting nervous, also… You do not even need to spell the type, the compiler is inferring the types for you and verifies them.

This is why most of the bugs are caught at compile time. and also why the compiler phase is longer.

Now, this is a blessing, but this is also a curse when  beginning. because you cant seem to see the end of it.

two things makes it even more painful:

- the compiler gives messages which are weird at first. once you know how to read them, it gets much better. we will do some mistakes on purpose to get acquainted.

- the mix and match of functions and actions breaks the type system. because this separation of concern is not present in other language, it is a new skills we need to work out, we will do it  when refactoring. just putting a print in the middle of a function for debug purpose can lead you to Monad Hell.