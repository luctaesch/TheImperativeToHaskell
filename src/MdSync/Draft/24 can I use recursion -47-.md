Yes.

lets use a classical , the factorial

reminder : 5! = 5x4x3X2x1 = 120

in C: 

using a for loop :

long factorial(int n)

{

  int c;

  long result = 1;

 

  for (c = 1; c <= n; c++)

    result = result * c;

 

  return result;

}

using recursion :

long factorial(int n)

{

  if (n == 0)

    return 1;

  else

    return(n * factorial(n-1));

}

in Haskell, using recursion :

fac (n) = if ( n == 0 ) then 1 else n*fac(n-1)