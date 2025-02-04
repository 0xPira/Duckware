# Title 
###### Solved by @Author
> This is a CTF about [Vuln Type 1, Vuln Type2 & Vuln Type 3]
## About the Challenge
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
## Solution

Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. [Nemo enim](instagram.com/duckwareteam/) ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit


![This is an alt text.](/images/example.jpg "This is a sample image")

sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet:

```
//Initialize the array that will hold the primes
var primeArray = [];
/*Write a function that checks for primeness and
pushes those values to the array*/
function PrimeCheck(candidate){
  isPrime = true;
  for(var i = 2; i < candidate && isPrime; i++){
    if(candidate%i === 0){
      isPrime = false;
    } else {
      isPrime = true;
    }
  }
  if(isPrime){
    primeArray.push(candidate);
  }
  return primeArray;
}
/*Write the code that runs the above until the
length of the array equals the number of primes
desired*/

var numPrimes = prompt("How many primes?");

//Display the finished array of primes

//for loop starting at 2 as that is the lowest prime number keep going until the array is as long as we requested
for (var i = 2; primeArray.length < numPrimes; i++) {   
    PrimeCheck(i); //
}
console.log(primeArray);
```



> So, we get the flag `DCK{FL_4G}`

