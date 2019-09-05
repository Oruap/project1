Required Outcome:

1.You must complete the code and run it to find out the following:
a.How many trials it will take you to break the one-way property using the brute-force method? You should repeat your experiment at least 5 timesand report your average number of trials. 
b.How  many  trials  it  will  take  you  to  break  the  collision-free  propertyusing  the brute-force method? Similarly, you should report the average.

2.You must demo your code and answer questions based on it. 

1.Brute force:One-Wayproperty breakThe  program's  objective  is  to  hit  a  "target"  hash  value  by  generating  the  hash  for all  possible combinations of different strings and matching it with the target hash value. The approach to generate strings and match them against a target is implemented as follows: 
1.Start with string length 1 
2.Generate all possible combinations of strings for current length using the character set, generate its hash and compare it with the target hash. 
3.If a match is found, the execution stops and reports the number of iterations used. 
4.If no match is found in all possible strings of current length, increment length by ‘1’ and go to step (2

The brute force code is used in the one-wayproperty break program oneway.cto generate strings In a systematic manner, exhausting all possibilities for a given length (starting with 1), and incrementing the length if no match was found.The oneway.cshouldbe executed a minimum of five times to find out the average number of iterations required to match the target hash.

2.Bute force:
Collision-Free property breakIn the case of collision free property, there is no restriction on target hash. The approach followed in the collision.c program to break this property is as follows: 
1.Allocate an array for saving hash values 
2.Generate initial message (call it M) 
3.Find M’s hash 
4.Generate random string S and find S’shash 
5.Compare S’s hash to M’s hash, if a match is found then exit and report the number of iterations used.
6.Compare S’s hash to each hash value in array, if any match is found then exit and report the number of iterations used. 
7.If no match is found, save the S’s hash into the array and go to step (4) 

To  break  the  collision  free  property,  you  just  need  to  find two  messages  with  matching  hash values. Matching the random string’s hash value to an initial hash as well as saved hash value (in the array) increases the probability of finding hash value with less number of iterations. 
Execute  the collision.c program  five  times  to  find  the  average  number  of iterationsrequired
