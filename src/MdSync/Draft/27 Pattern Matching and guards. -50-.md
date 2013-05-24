Pattern Matching .

remember the factorial definition ?

fac n = if ( n == 0 ) then 1 else n*fac(n-1)

it could also be written like :

fac 0 =  1 

fac n =  n*fac(n-1)

the parameters will be tried to be matched on the first equation, and if failed, the next one is tried; ( which is what (if ( n ==0 ) then .. else ) is doing…)

if no match is found, an error is raised. _ is a wildcard, and can be use to catch anything.