Watch this video to understand what to do in this exercise block [link](https://www.youtube.com/watch?v=zGpplZj4zY0&feature=youtu.be)

#### Getting To Know String Methods

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) and look for the name of method to learn about it.

**Write in your own way of understanding (don't copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (4-5 times to understand)
2. Data types of parameters
3. Return value type
4. Write three examples
5. In your own words and one sentence explain what this method does.

Example:

1. `charAt`

   - Parameter: (index) defaults to 0 - (number data type)
   - Return: character at specific index in the string (string data type)
   - Example:
     ```js
     let name = 'Arya Stark';
     name.charAt(2); //"y"
     let sentance = 'A quick brown fox jumped over a lazy dog';
     sentance(4); // "i"
     let houseName = 'Starks';
     houseName.charAt(0); // "S"
     ```
   - `charAt` accepts a index (number data type) and return the character on that index in the string.

2. `toUpperCase`
  
   - Parameter: toUpperCase
   - Return: A new string representing the calling string converted to upper case.
   - Example:
     ```js
     let name = 'Aegon Targaryen';
     name.toUpperCase(); //"AEGON TARGARYEN"
     let houseName = 'Targaryen';
     houseName.toUpperCase(); // "TARGARYEN"
     let sentence = 'Lives in Winterfell';
     sentence.toUpperCase(); // "LIVES IN WINTERFELL"
     ```
   - `toUpperCase`  It is very straight to convert any value to into uppercase we say "toUpperCase" & call this method and we get uppercase. 

3. `toLowerCase`
  
   - Parameter: toLowerCase
   - Return: A new string representing the calling string converted to upper case.
   - Example:
     ```js
     let name = 'Aegon Targaryen';
     name.toLowerCase(); //"aegon targaryen"
     let houseName = 'Targaryen';
     houseName.toLowerCase(); // "targaryen"
     let sentence = 'Lives in Winterfell';
     sentence.toLowerCase(); // "lives in winterfell"
     ```
   - `toLowerCase`  It is very straight to convert any value to into LowerCase we say "toLowerCase" & call this method and we get LowerCase. 

4. `trim`
  
   - Parameter: The trim method removes whitespace from both ends of a string.
   - Return: A new string representing stripped of whitespace from both its beginning and end.
   - Example:
     ```js
     let name = '    Aegon     Targaryen   ';
     name.trim(); //"Aegon Targaryen"
     let houseName = '    Targaryen     ';
     houseName.trim(); // "Targaryen"
     let sentence = '      Lives   in    Winterfell       ';
     sentence.trim(); // "lives in winterfell"
     ```
   - `trim`  We have a variable and that contain some extra space in start & in last & if we access thaat value we will see there are some extra spaces what if we want to trim the value so for that we will say ".trim" it will remove all the white spaces from the start and end    

5. `trimEnd`

   - Parameter: The trim method removes whitespace from end of a string.
   - Return: A new string representing stripped of whitespace from its end.
   - Example:
     ```js
     let name = '    Aegon     Targaryen   ';
     name.trimEnd(); //"     Aegon     Targaryen"
     let houseName = '    Targaryen     ';
     houseName.trimEnd(); // "     Targaryen"
     let sentence = '      Lives   in    Winterfell       ';
     sentence.trimEnd(); // "      Lives   in    Winterfell"
     ```
   - `trimEnd`  We have a variable and that contain some extra space in last & if we access that value we will see there are some extra spaces what if we want to trim the value so for that we will say ".trimEnd" it will remove all the white spaces from the end.  

6. `trimStart`

   - Parameter: The trim method removes whitespace from end of a string.
   - Return: A new string representing stripped of whitespace from its end.
   - Example:
     ```js
     let name = '    Aegon     Targaryen   ';
     name.trimStart(); //'Aegon     Targaryen   '
     let houseName = '    Targaryen     ';
     houseName.trimStart(); // "Targaryen     "
     let sentence = '      Lives   in    Winterfell       ';
     sentence.trimStart(); // "Lives   in    Winterfell      "
     ```
   - `trimStart`  We have a variable and that contain some extra space in start & if we access that value we will see there are some extra spaces what if we want to trim the value so for that we will say ".trimStart" it will remove all the white spaces from the start.  

7. `concat`

   - Parameter: One or more strings to concatenate to str.
   - Return:A new string containing the combined text of the strings provided.
   - Example:
     ```js
     let firstName = 'Aegon';
     let lastName = 'Targaryen';
     firstName.concat(' ', lastName); //'Aegon Targaryen'
     let name1 = "John";
     let name2 = "Snow";
     name1.concat(' ', name2); //'John Snow';
     let sentence1 = 'Lives';
     let sentence2 = 'in';
     let sentence3 = 'Winterfell';
     sentence1.concat(' ', sentance2, sentence3); // "Lives in Winterfell "
     ```
   - `concat` Concat method is used to concatinating multiple string values. 

8. `endsWith`

   - Parameter:The characters to be searched for at the end .
   - Return: true if the given characters are found at the end of the string; otherwise, false.
   - Example:
     ```js
    let name = 'Aegon Targaryen';
     name.endsWith('yen'); //"true"
     let houseName = 'Targaryen';
     houseName.endsWith('ar'); // "false"
     let sentence = 'Lives in Winterfell';
     sentence.endsWith('all'); // "true"
     ```
   - `endsWith` endwith return true or false based on whether that string ends with specific character or not.

9. `includes`

   - Parameter: The characters to be searched in between the string .
   - Return: true if the given characters are found in the string; otherwise, false.
   - Example:
     ```js
    let name = 'Aegon Targaryen';
     name.includes('Aegon'); //"true"
     let houseName = 'Targaryen';
     houseName.includes('AR'); // "false"
     let sentence = 'Lives in Winterfell';
     sentence.includes ('Winterfell'); // "true"
     ```
   - `includes` true if the search string is found anywhere within the given string; otherwise, false if not.

10. `indexOf`

   - Parameter: it accepts search value.
   - Return: The index of the first occurrence of searchValue, or -1 if not found.
   - Example:
     ```js
    let name = 'Aegon Targaryen';
     name.indexOf('T'); // 6
     let houseName = 'Targaryen';
     houseName.indexOf('AR'); // -1
     let sentence = 'Lives in Winterfell';
     sentence.indexOf (' '); // 5
     ```
   - `indexOf` Index of  return the index of specific character that you are looking for.
   
11. `lastIndexOf`

   - Parameter: it accepts search value.
   - Return: The index of the last occurrence of searchValue; if not found it will give -1.
   - Example:
     ```js
    let name = 'Daenerys Targaryen';
     name.lastIndexOf('T'); // 6
     let houseName = 'Targaryen';
     houseName.lastIndexOf('AR'); // -1
     let sentence = 'Lives in Westros';
     sentence.lastIndexOf (' '); // 8
     ```
   - `lastIndexOf` Index of  return the index of specific character that you are looking for.
   
12. `padEnd`

   - Parameter: it accepts ' padEnd(targetLength) ' to add padding in the end.
   - Return: A String of the specified targetLength with the padString applied at the end of the current str.
   - Example:
     ```js
    let name = 'Aegon Targaryen';
     name.padEnd('26'); // 'Aegon Targaryen           '
     let houseName = 'Targaryen';
     houseName.padEnd('18'); // 'Targaryen         '
     let sentence = 'Lives in Winterfell';
     sentence.padEnd ('25'); // 'Lives in Winterfell      '
     ```
   - `padEnd`  This padEnd used to add some padding at the end.
  
13. `padStart`

 - Parameter: it accepts ' padStart(targetLength) ' to add padding in the start.
   - Return: A String of the specified targetLength with the padString applied at the start of the current str.
   - Example:
     ```js
    let name = 'Aegon Targaryen';
     name.padStart('26'); // '           Aegon Targaryen'
     let houseName = 'Targaryen';
     houseName.padStart('18'); // '         Targaryen'
     let sentence = 'Lives in Winterfell';
     sentence.padStart ('10'); // '      Lives in Winterfell'
     ```
   - `padStart`  This padStart used to add some padding at the end.

14. `repeat`

 - Parameter: It will repeat the same string for multiple time. 
   - Return: A new string containing the specified number of copies of the given string.
   - Example:
     ```js
    let name = 'Aegon Targaryen ';
     name.repeat('4'); //'Aegon Targaryen Aegon Targaryen Aegon Targaryen Aegon Targaryen '
     let houseName = 'Targaryen';
     houseName.repeat('6'); // ' Targaryen Targaryen Targaryen Targaryen Targaryen Targaryen'
     let sentence = 'Lives in Winterfell ';
     sentence.repeat ('3'); // 'Lives in Winterfell Lives in Winterfell Lives in Winterfell '
     ```
   - `repeat` A new string containing the specified number of copies of the given string.

15. `replace`

 - Parameter: It will replace the same string with another string.
   - Return: A new string, with some or all matches of a pattern replaced by a replacement.
   - Example:
     ```js
    let name = 'Aegon Targaryen ';
     name.replace('Aegon', 'John'); //'John Targaryen '
     let houseName = ' Targaryen';
     houseName.replace('', 'Daenerys'); //'Daenerys Targaryen'
     let sentence = 'Lives in Winterfell ';
     sentence.replace ('Winterfell', 'Westros'); // 'Lives in Westros '
     ```
   - `repeat` So replace is used to replace a new string with old one. 

16. `slice`
- Parameter: it takes begin index and second one is end index from where slicing will start
- Return: It returns new string after slcing
- Example:
 ```js
    let name = 'Aegon Targaryen ';
     name.slice('4', '12'); //'n Targar'
     let houseName = ' Targaryen';
     houseName.slice('3', '8'); //'rgary'
     let sentence = 'Lives in Winterfell ';
     sentence.slice ('4', '18'); //'s in Winterfel'
     ```
 - `slice` slice it gives sliced string.

// 17. `split`
// - Parameter: it takes two parameter both are optional,first one is seprator by which string has to be separated,second one is limit means - array
// - Return: It returns array of string
// - Example:
 
// -  split it gives splitted array of strings. it split the strings at each seprator given
18. `substring`

 