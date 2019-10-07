
Description

In the last challenge, you searched for the word "Hello"using the regular expression /Hello/. That regex searched for a literal match of the string "Hello". Here's another example searching for a literal match of the string "Kevin":

let testStr = "Hello, my name is Kevin.";
let testRegex = /Kevin/;
testRegex.test(testStr);
// Returns true
Any other forms of "Kevin"will not match. For example, the regex /Kevin/will not match "kevin"or "KEVIN".

let wrongRegex = /kevin/;
wrongRegex.test(testStr);
// Returns false
A future challenge will show how to match those other forms as well.


challenge

Complete the regex waldoRegexto find "Waldo"in the string waldoIsHidingwith a literal match.


Tests
- Your regex waldoRegexshould find "Waldo"
- Your regex waldoRegexshould not search for anything else.
- You should perform a literal string match with your regex.


Seeds

let waldoIsHiding = "Somewhere Waldo is hiding in this text.";
let waldoRegex = /search/; // Change this line
let result = waldoRegex.test(waldoIsHiding);


Solution

let waldoIsHiding = "Somewhere Waldo is hiding in this text.";

let waldoRegex = /Waldo/; // Change this line

let result = waldoRegex.test(waldoIsHiding);
