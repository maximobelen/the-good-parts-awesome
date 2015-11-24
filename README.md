# the-good-parts-awesome

##Motivation
<br>
Every time when you start to learn a programming language, guys who know about the language or who don't know a shit but try to look like they know suggest you a lecture and article or a book. Well when I started to learn Javascript I heard many times did you read The Good Parts - Douglas Crockford ?? And I said every time: NO, I didn't read it!! But finally I decided to read this amazing book!
Now I want to make a summary of the things that I really keep with me after reading this awesome book.

For the ones that don't know (and are in the same situations I was before)...  this is the book I'm talking:
<br>  
<br>
<div style="text-align:center"><img src ="./assets/images/cover.png" /></div>
<br>
<br>
##Chapters
1. Good Parts
2. Grammar 
3. Objects 
4. Functions 
5. Inheritance
6. Arrays
7. Regular Expressions
8. Methods 
9. Style 
10. Beautiful Features

<br>
##Summary
###1. Good Parts
I can't sum up this part, just read the awesome introduction of Douglas Crockford.
###2. Grammar 
###3. Objects 
###4. Functions 
###5. Inheritance
###6. Arrays
As we know arrays are linear allocation on memory which each elements are accessed by intergers that allow you to compute offset but...<br>
In Javacript arrays are not the same as in another language. In Javascript arrays are objects that has some array-like characteristics, this make arrays significantly slower than a real array.
###7. Regular Expressions
Take care with two lines, in a JavaScript program, the regular expression must be on a single line!
###8. Methods 
####Arrays
#####Don't confuse splice with slice
#####Sorting Arrays
Sorting numbers with array.sort() didn't works as we expect.<br><br>
If you have this array:<br>
var n = [4, 8, 15, 16, 23, 42]; <br>
and use n.sort();<br><br>
you are going to get:<br>
// n is [15, 16, 23, 4, 42, 8]<br><br>
JavaScript’s default comparison function assumes that the elements to be sorted are strings.<br>
So take care of this! You have to create you own function to order numbers, in the book Douglas Crockford suggest one solution.
#####Shift
The shift method removes the first element from an array and returns it.<br>
Avoid using shift, is slower that pop. In the book Douglas suggest us to implemented in this way:<br><br>
Array.method('shift', function () { return this.splice(0, 1)[0];});

####Strings
#####Concat
var s = 'C'.concat('a', 't'); // s is 'Cat'<br>
Concat a string with this method is the same as concating with + operator in this way:<br>
var s = 'C' + 'a' + 't';<br>

This last one is more clearly to read than the concat.

#####toLocaleLowerCase() and toLocaleUpperCase() are nice methods
Some months ago I worked on a turkish project and in some place we have to put all the text in uppercase, as I didn't know about the existence of this method I used the normal string.toUpperCase(), but we loose the real character. If you use toLocaleUpperCase() language ‘i’ converts to ‘&#x130;’, not ‘I’ same with the inverted convertion.

###9. Style 
###10. Beautiful Features
Also I don't want to sum up this part, please take a look on the conclusions of Douglas Crockford.

<br>
##Personals Conclusions
<br>
##Feel free to contribute so we can create a real awesome summary :)