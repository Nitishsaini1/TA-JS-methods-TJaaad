Watch this video to understand what to do in this exercise block [link](https://www.youtube.com/watch?v=zGpplZj4zY0&feature=youtu.be)

## Getting To Know Array Methods

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) and look for the name of method to learn about it.

**Write in your own way of understanding (don't copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (2-3 times to understand)
2. Data types of parameters
3. Return value type
4. Write three examples
5. In your words what this method does.
6. Does it mutate the original value or not (check https://doesitmutate.xyz)

Example:

1. `concat`

   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: a single Array consisting of by all the values passed as parameters in the same order.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.concat(4); //[1,2,3,4]
     let sentanceArray = 'A quick brown fox jumped over a lazy'.split(' ');
     sentanceArray.concat('dog').join(' '); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.concat('black', 'red', 21, true); // ['red','green','blue','black', 'red', 21, true]
     ```
   - `concat` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

2. `join`

   - Parameter: It accepts only seprator and optional.
   - Return: A string with all array elements joined. If arr.length is 0, the empty string is returned.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.join(4); //['14243']      
     let colors = ['red', 'green', 'blue'];
     colors.join(''); // 'redgreenblue' 
     colors.join();   // 'red,green,blue'
     colors.join(', ');  // 'red, green, blue'
     colors.join(' + '); //'red + green + blue'
     ```
   - `join` The `join()` method joins all elements of an array into a string. It does not change the original array.
   - No it does not mutate the original array


3. `flat`

   - Parameter:  It accepts only depth and optional.
   - Return: it returns array with sub-array elements concatenated into it.
   - Example:
     ```js
     let numbers = [1, 2, [3, 4, [5, 6]]];
     numbers.flat(); //[1,2,3,4, Array(2)]
     numbers.flat(0); //[1,2, Array(3)]
     numbers.flat(6); //[1,2,3,4,5,6]      
     ```
   - `flat` Flat accepts one parameter that defines what did they make it flat. It does not change the original array.
   - No it does not mutate the original array


4. `push`

   - Parameter: The element(s) to add to the end of the array.
   - Return:The new length property of the object upon which the method was called.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.push(4); // 4
     let sentanceArray = 'A quick brown fox jumped over a lazy';
     sentanceArray.push('dog') ; // 2
     let colors = ['red', 'green', 'blue'];
     colors.push('black', 'red', 21, true); //  7
     ```
   - `push` The push method adds one or more elements to the end of an array and returns the new length of the array.
   - Yes it mutate the original array


5. `indexOf`

   - Parameter: index number of element in the array.
   - Return: The first index of the element in the array; -1 if not found.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.indexOf(3); // 2 
     let sentanceArray = ['A quick brown fox jumped over a lazy'];
     sentanceArray.indexOf('dog'); // -1
     let colors = ['red', 'green', 'blue'];
     colors.indexOf('red'); // 0
     colors.indexOf('green'); // 1
     colors.indexOf('blue'); // 2
     ```
   - `indexOf`The indexOf method returns the first index at which a given element can be found in the array, or -1 if it is not present.
   - No it does not mutate the original array


6. `lastIndexOf`


   - Parameter: index number of element in the array.
   - Return: The last index of the element in the array; -1 if not found.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.lastIndexOf(3); // 2 
     let sentanceArray = ['A quick brown fox jumped over a lazy'];
     sentanceArray.lastIndexOf('dog'); // -1
     let colors = ['red', 'green', 'blue'];
     colors.lastIndexOf('red'); // 0
     colors.lastIndexOf('green'); // 1
     colors.lastIndexOf('blue'); // 2
     ```
   - `lastIndexOf` The lastIndexOf() method returns the last index at which a given element can be found in the array, or -1 if it is not present. The array is searched    backwards, starting at fromIndex.
   - No it does not mutate the original array

7. `includes`

   - Parameter: The value to search for.
   - Return:   returning true or false if it present in the array.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.includes(2); // true
     let sentanceArray = ['A quick brown fox jumped over a lazy' ];
     sentanceArray.includes('dog'); // false
     let colors = ['red', 'green', 'blue'];
     colors.includes('green' ); //  true
     colors.includes('black' ); //  false
     ```
   - `includes`The includes() method determines whether an array includes a certain element, returning true or false as appropriate.
   - No it does not mutate the original array


8. `reverse`

   - Parameter: It accepts no parameter.
   - Return: Returns the reversed array.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.reverse(); //[3, 2, 1]
     let colors = ['red', 'green', 'blue'];
     colors.reverse(); // ['blue', 'green', 'red']
     ```
   - `reverse` The reverse() method reverses an array in place. The first array element becomes the last, and the last array element becomes the first.
   - Yes it mutate the original array


9. `every`
   - Parameter:The every() method tests whether all elements in the array pass the test implemented by the provided function.
   - Return:  if the callbackFn function returns a truthy value for every array element. Otherwise, false.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     let check = numbers.every(
       function(number){
          return number > 0;
       }
     ) 
    console.log(check) // true

     let numbers = [1, 2, 3];
     let check = numbers.every(
       function(number){
          return number > 2;
       }
     ) 
    console.log(check) // false
    
     ```
   - `every` The every() method tests whether all elements in the array pass the test implemented by the provided function.
   - No it does not mutate the original array


10. `shift`
   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: a single Array consisting of by all the values passed as parameters in the same order.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.concat(4); //[1,2,3,4]
     let sentanceArray = 'A quick brown fox jumped over a lazy'.split(' ');
     sentanceArray.concat('dog').join(' '); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.concat('black', 'red', 21, true); // ['red','green','blue','black', 'red', 21, true]
     ```
   - `concat` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array


11. `forEach`
   - Parameter:accept callback function which accept 4 parameters
   - Return: new array of each element resulted from callback function
   - Example:
     ```js
     let colors = ["black", "blue", "brown", "green"];
     ler allColors = "";
     colors.forEach(forEachColor);
     function forEachColor(color){
       allColor += color + " ";
     }
     console.log(allColors);
     ```
   -`map` it takes call back function and  execute each element for callback function.
   - No it does not mutate the original array 

12. `find` 


13. `unshift` 

14. `findIndex` 

15. `filter` 

16. `flat` 

17. `forEach` 

18. `map` 

19. `pop` 

20. `reduce` 

21. `slice` 

22. `some`
  
