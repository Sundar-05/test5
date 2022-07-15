# Javascript cheatsheet

<img src="images/IDSNlogo.png" width="200">

<table>
<tr>
<th width="20%">Item</th width="20%"><th>Syntax</th><th width="40%">Description</th><th width="20%">Example</th>
</tr>

<tr>
<td width="20%">Declaring Variables<br>var, let, const </td><td width="20%"><code>let &lt var_name &gt = &lt value &gt; </code>
<td width="40%">
<b>var</b> - global access, value can chage<br/>
<b>let</b> - access within block where it is declared, value can change<br/>
<b>const</b> - access within block where it is declared, value cannot change
</td>
<td width="20%">
<code>let i = 5;</code><br/>
<code>var myStr = "John";</code><br/>
<code>const pi = 3.14 </code></td>
</tr>

<tr>
<th colspan="4">Strings</th>
</tr>

<tr>
<td width="20%">
length
</td>
<td width="20%">
<code><i>string_obj</i>.length</code>
</td>
<td width="20%">
<b>length</b> Returns the length of the string
</td>
<td width="20%">
<code>let myStr = "Hello";
console.log(myStr.length);
</code>
<br/>
Output is 5
</td>
</tr>

<tr>
<td width="20%">
split
</td>
<td width="20%">
<code><i>string_obj</i>.split(<i>separator</i>)
</code>
</td>
<td width="20%">
<b>split</b> Splits the string based on the separator and returns an array. 
</td>
<td width="20%">
<code>let myStr = "Hello! How are you?";
console.log(myStr.split())
</code>
<br/>
Output is [ 'Hello!', 'How', 'are', 'you?' ]
</td>
</tr>

<tr>
<td width="20%">
charAt
</td>
<td width="20%">
<code><i>string_obj</i>.charAt(<i>index</i>)
</code>
</td>
<td width="20%">
<b>charAt</b> returns the character at a specified index in a string. Index starts at 0 ends at length-1
</td>
<td width="20%">
<code>let myStr = "Hello";<
console.log(myStr.charAt(0))
</code>
<br/>
Output is H
</td>
</tr>

<tr>
<td width="20%">
replace
</td>
<td width="20%">
<code><i>string_obj</i>.replace(<i>"SearchValue","NewValue"</i>)
</code>
</td>
<td width="20%"> 
<b>replace</b> searches a string for a specified value, or a regular expression, and returns a new string where the specified values are replaced.
</td>
<td width="20%">
<code>let myStr = "Hello User";
console.log(myStr.replace("User","World"));
</code>
<br/>
Output is Hello World
</td>
</tr>

<tr>
<td width="20%">
substring
</td>
<td width="20%">
<code><i>string_obj</i>.substring(start, end)
</code>
</td>
<td width="20%">
<b>substring</b> is used to extract characters, between to indices from the given string, and returns the substring. It excludes the last index
</td>
<td width="20%">
<code>let myStr="Hello";
console.log(myStr.substing(1,4));
</code> <br/>
Output is ell
</td>
</tr>

<tr>
<td width="20%">
startswith
</td>
<td width="20%">
<code><i>string_obj</i>.startsWith(searchvalue)
</code>
</td>
<td width="20%">
<b>startsWith</b> returns true if a string begins with a specified string, otherwise false
</td>
<td width="20%">
<code>let myStr="Hello from the other side";
console.log(myStr.startsWith("Hello"));
</code> <br/>
Output is <i>true </i>
</td>
</tr>

<tr>
<td width="20%">
endsWith
</td>
<td width="20%">
<code><i>string_obj</i>.endsWith(searchvalue))
</code>
</td>
<td width="20%">
<b>endsWith</b> returns true if a string ends with a specified string, otherwise false
</td>
<td width="20%">
<code>let myStr="Hello from the other side";
console.log(myStr.startsWith("side"));
</code> <br/>
Output is <i>true </i>
</td>
</tr>

<tr>
<td width="20%">
toUpperCase
</td>
<td width="20%">
<code><i>string_obj.</i>toUpperCase()
</code>
</td>
<td width="20%">
<b>toUpperCase</b> converts a string to uppercase letters
</td>
<td width="20%">
<code>let myStr="hello";
console.log(myStr.toUpperCase());
</code> <br/>
Output is HELLO
</td>
</tr>

<tr>
<td width="20%">
toLowerCase
</td>
<td width="20%">
<code><i>string_obj.</i>toLowerCase()
</code>
</td>
<td width="20%">
<b>toLowerCase</b> converts a string to lowercase letters
</td>
<td width="20%">
<code>let myStr="HELLO";
console.log(myStr.toUpperCase());
</code> <br/>
Output is hello
</td>
</tr>

<tr>
<td width="20%">
concat
</td>
<td width="20%">
<code><i>string_obj.</i>concat(<i>string1, string2,..,stringN</i>)
</code>
</td>
<td width="20%">
<b>concat</b> joins two or more strings.
</td>
<td width="20%">
<code>let myStr="Hello";
let str="World";
console.log(myStr.concat(str));
</code> <br/>
Output is HelloWorld
</td>
</tr>

<tr>
<th colspan="4">Arrays</th>
</tr>
<tr>
<td width="20%">
push
</td>
<td width="20%">
<code><i>arr_name.</i>push(<i>value</i>)
</code>
</td>
<td width="20%">
<b>push</b> adds new items to the end of an array.
</td>
<td width="20%">
<code>let myArr=["Hello"];
myArr.push("World");
console.log(myArr);
</code> <br/>
Output is ["Hello","World"]
</td>
</tr>

<tr>
<td width="20%">
pop
</td>
<td width="20%">
<code><i>arr_name.</i>pop()
</code>
</td>
<td width="20%">
<b>pop</b> removes the last element of an array.
</td>
<td width="20%">
<code>let myArr=["Hello","World"];
myArr.pop();
console.log(myArr);
</code> <br/>
Output is ["Hello"]
</td>
</tr>

<tr>
<td width="20%">
length
</td>
<td width="20%">
<code><i>arr_name.</i>length
</code>
</td>
<td width="20%">
<b>length</b> sets or returns the number of elements in an array.
</td>
<td width="20%">
<code>let myArr=["Hello","World"];
console.log(myArr.length);
</code> <br/>
Output is 2
</td>
</tr>


<tr>
<td width="20%">
indexOf
</td>
<td width="20%">
<code><i>arr_name.</i>indexOf(<i>item</i>)
</code>
</td>
<td width="20%">
<b>indexOf</b> searches for a specified item and returns its position.
</td>
<td width="20%">
<code>let myArr=["Hello","World"];
console.log(myArr.indexOf("World")
</code> <br/>
Output is 1
</td>
</tr>

<tr>
<td width="20%">
lastIndexOf
</td>
<td width="20%">
<code><i>arr_name.</i>lastIndexOf(<i>item</i>)
</code>
</td>
<td width="20%">
<b>lastIndexOf</b> returns the last index (position) of a specified value.
</td>
<td width="20%">
<code>let myArr=["Hello","World","Hello"];
console.log(myArr.lastIndexOf("Hello");
</code> <br/>
Output is 2
</td>
</tr>

<tr>
<td width="20%">
entries
</td>
<td width="20%">
<code><i>arr_name.</i>entries()
</code>
</td>
<td width="20%">
<b>entries</b> Returns and Array Iterator that helps you to iterate through the array and recieve each entry as an array of two elements containing the key and the value, where in the key is the index position of the element and value is the element itself.
</td>
<td width="20%">
<code>const hello = ["h", "e", "l", "l","o"];
console.log(hello.entries());
</code>
<br/>
Output is 
Object [Array Iterator] {}


<td width="20%">
</td>
</tr>

<tr>
<td width="20%">
find
</td>
<td width="20%">
<code>Array.find(&lt;arrElemet&gt;=>{
    //return boolean based on a condition
}
</code>
</td>
<td width="20%">
<b>find</b> Finds the first occurance of an element in the array which returns true on checking the condition
</td>
<td width="20%">
<code>//Find the first string with s
let myarr = ["Mercury","Venus","Earth","Mars"];
let found = myarr.find(val=>{
    return val.includes("s");
})
console.log(found);
</code>
<br/>
Output Venus
</td>
</tr>

<tr>
<td width="20%">
filter
</td>
<td width="20%">
<code>Array.filter(&lt;arrElemet&gt;=>{
    //return boolean based on a condition
}
</code>
</td>
<td width="20%">
<b>filter</b> Finds the all occurances of elements in the array which returns true on checking the condition
</td>
<td width="20%">
<code>//Find the all strings with s
let myarr = ["Mercury","Venus","Earth","Mars"];
let found = myarr.filter(val=>{
    return val.includes("s");
})
console.log(found);
</code>
<br/>
Output [Venus,Mars]
</td>
</tr>

<tr>
<td width="20%">
map
</td>
<td width="20%">
<code>Array.map(&lt;arrElemet&gt;=>{
    //return processed value
}
</code>
</td>
<td width="20%">
<b>map</b> Processes the all elements of the array which returns a new processed array of same size
</td>
<td width="20%">
<code>let myarr = ["name","place","thing","animal"];
let found = myarr.map(val=>{
    return val+"s";
})
console.log(found);
<br/>
Output [ 'names', 'places', 'things', 'animals' ]
</td>
</tr>

<tr>
<td width="20%">
concat
</td>
<td width="20%">
<code><i>arr_name.</i>.concat(arr1.name);
</code>
</td>
<td width="20%">
<b>concat</b> concatenates (joins) two or more arrays.
</td>
<td width="20%">
<code>let hello = ["hello", "world" ];
let lorem = ["along","lorem"]
let h = hello.concat(lorem);
console.log(h);
</code>

Output is 
 ["hello", "world", "along", "lorem"]
<td width="20%">
</td>
</tr>

<tr>
<th colspan="4">Map</th>
</tr>
<tr>
<td width="20%">
set
</td>
<td width="20%">
<code>mapName.set(key,value);
</code>
</td>
<td width="20%">
<b>set</b> helps you define a new element with akey and its value
</td>
<td width="20%">
<code>var newMap = new Map();
newMap.set("h", 1);
console.log(newMap);
</code><br/>
Output is {"h" => 1}
</td>
</tr>

<tr>
<td width="20%">
get
</td>
<td width="20%">
<code>mapName.get(key);
</td>
<td width="20%"><b>get</b> helps you return a value of key you are searching for
</td>
<td width="20%">
<code>var newMap = new Map();
newMap.get("h");
console.log(newMap);
</code><br/>
Output is {"h" => 1}
</td>
</td>
</tr>

<tr>
<td width="20%">
keys
</td>
<td width="20%">
<code>mapName.keys();
</code>
</td>

<td width="20%"> 
<b>get</b> is used to get all of the keys associated with the mapName
</td>
<td width="20%">
<code>var newMap = new Map();
newMap.set("h",1);
newMap.set("i",2);
console.log(newMap.keys());
</code><br/>
Output is {"h", "i"}
</td>
</tr>

<tr>
<td width="20%">
values
</td>
<td width="20%">
<code> mapName.values();
</code>
</td>
<td width="20%"><b>values</b> is used to get all of the values to the keys associated with the mapName
</td>
<td width="20%"> 
<code>var newMap = new Map();
newMap.set("h",1);
newMap.set("i",2);
console.log(newMap.values());
</code><br/>
Output is {1,2}
</td>
</tr>

<tr>
<td width="20%">
has
</td>
<td width="20%">
<code>mapName.has(key_name);
</code>
</td>
<td width="20%"><b>has</b> is used to check if the key passed resides in the map or not,  and returns true or false
</td>
<td width="20%">
<code>var newMap = new Map();
newMap.set("h",1);
newMap.set("i",2);
console.log(newMap.has(i));
</code><br/>
Output is true
</td>
</tr>

<tr>
<td width="20%">
delete
</td>
<td width="20%">
<code>mapName.delete(key_name);
</code>
</td>
<td width="20%"><b>delete</b> is used to delete the key and the value from the map
</td>
<td width="20%">
<code>var newMap = new Map();
newMap.set("h",1);
newMap.set("i",2);
newMap.delete("h");
console.log(newMap);
</code><br/>
Output is {"i" => 2}
</td>
</tr>

<tr>
<th colspan="4">JSON</th>
</tr>
<tr>
<td width="20%">
Create JSON
</td>
<td width="20%">
<code>let varname={name1:value1,name2:values2,.....}
</code>
</td>
<td width="20%">
JSON is a dictionary Object with Key-Value pairs. 
</td>
<td width="20%">
<code>let myjson1={};
let myjson2 = {"name":"Jennifer","age":"32"}
</code>
</td>
</tr>

<tr>
<td width="20%">
Add entry to JSON
</td>
<td width="20%">
<code>let jsonObj[&lt;key&gt;]=&lt;value&gt;
</code>
</td>
<td width="20%">
Adds an entry to JSON Object mapping the key to value
</td>
<td width="20%">
<code>let myjson1 = {};
myjson1["name"]="Jason";
console.log(myjson1);
</code>
</td>
</tr>

<tr>
<th colspan="4">Operators</th>
</tr>

<tr>
<td width="20%">
Arithmetic
</td>
<td width="20%">
<code> &lt;Operand1&gt; &lt;Operator&gt; &lt;Operand2&gt;
</code>
</td><td width="20%">
<b>+</b> addition <br/>
<b>-</b> subtration<br/>
<b>/</b> division<br/>
<b>*</b> multiplication<br/>
<b>%</b> modulus(gives remainder)<br/>
<b>++</b> increment by 1<br/>
<b>--</b> decrement by 1<br/>

</td><td width="20%">
<code>
let num1 = 2;
let num2 = 2;
console.log(num1+num2);
console.log(num1-num2);
console.log(num1/num2);
console.log(num1*num2);
console.log(num1%num2);
num1++;
console.log(num1);
num2--;
console.log(num1);
</code>
<br/>
Output is 4 0 1 4 0 3 3 


</td>
</tr>

<tr>
<td width="20%">
Logical
</td>
<td width="20%">
<code>condition1 && condition2
condition1 || condition2
! condition1
</code>
</td>
<td width="20%">

<b>&&</b> (AND)is used to check if all the operand conditions are true<br/>
<b>||</b> (OR)is used to check if either of the operand condition are true   <br/>
<b>!</b> (NOT) is used to check if the operand condition is not met  </td>
<td width="20%">
<code>let num1 = 12, num2 = 2;
console.log(num1>10 && num2>10);
console.log(num1>10 || num2>10);
console.log(!(num1==num2));
</code>
<br/>
Output is false true true

<td width="20%">
</td>
</tr>

<tr>
<td width="20%">
Assignment
</td>
<td width="20%">
<code>variable = value
variable += incremental value
variable -= decremental value
%= modulus value
/= divide value
*= multiply value
</code>
</td> <td width="20%">
<b>a=b </b>assigns the value of b to a <br/>
<b>a+=b</b> adds the value of b to a and stores it in a<br/>
<b>a-=b</b> subtracts the value of b from a and stores it in a<br/>
<b>a%=b</b> divides the value of a by b and stores the remainder in a<br/>
<b>a/=b</b> divides the value of a to b and stores the quotient in a<br/>
<b>a*=b</b> multiplies the value of a and b and stores the value in a<br/>

</td><td width="20%">
<code>let num1 = 12, num2 = 2;
console.log(num1=num2);
console.log(num1+=num2);
console.log(num1-=num2);
console.log(num1/=num2);
console.log(num1*=num2);
console.log(num1%num2);
console.log(num1=num2);
</code>
<br/>
Output is 2  14  10  6  24  0  2


</td>
</tr>

<tr>
<th colspan="4">Loops</th>
</tr>

<tr>


<td width="20%">
For Loop
</td>
<td width="20%">
<code>for(initialization;condition;increment/decrement){
    //code block
}
</code>
</td>
<td width="20%">

<b>for</b> loops throughout the block of code a number of times making sure the condition is satisfied 

</td>


<td width="20%">
<code>for(let num = 0 ; num <=5 ; num++){
    console.log(num)
}
</code> <br/>
Output is 0 1 2 3 4 5

</td>
</tr>

<tr>


<td width="20%">
while
</td>
<td width="20%">
<code>while(condition){
    //code block
}
</code>
</td>
<td width="20%">

<b>while</b> itrates through the block of code while a specified condition is true

</td>


<td width="20%">
<code>let num1 = 0;
let num2 = 5;
while(num1 < num2){ 
    console.log(num1) 
    num1++; 
}

</code> <br/>
Output is 0 1 2 3 4

</td>
</tr>

<tr>


<td width="20%">
do while
</td>
<td width="20%">
<code>do{ 
    //code block
}
while(condition)
</code>
</td>
<td width="20%">

<b>do while</b> loops throughout the block once before checking condition.

</td>


<td width="20%">
<code>let num = 5;
do {
    console.log(num);
    num--;
}

while(num > 0)

</code> <br/>
Output is 5 4 3 2 1

</td>
</tr>

<tr>


<td width="20%">
for in
</td>
<td width="20%">
<code>for (var in object) {
    //code block<br/>
}
</code>
</td>
<td width="20%">

<b>for in</b> is used to itrate through the specific property/type of the object 

</td>


<td width="20%">
<code>let arr = ["a","b","c"];
for(let i in arr) {
    console.log(arr[i]);
}

</code> <br/>
Output is a b c

</td>
</tr>


<tr>
<th colspan="4">Conditional statements</th>
</tr>

<tr>
<td width="20%">
if
</td>
<td width="20%">
<code>
if(<i>condition</i>){
    //code Block...
}
</code>
</td>
<td width="20%">
<b>if</b> a specified condition is true, a block of code will be executed
</td>
<td width="20%">
<code>let num = 5;
if(num = 5){
    console.log(true);
}
</code> <br/>
Output is true
</td>
</tr>

<tr>
<td width="20%">
if-else
</td>
<td width="20%">
<code>if(<i>condition</i>){
    //Code Block... 
} else {
    //Code Block...
}
</code>
</td>
<td width="20%">
<b>if</b> a specified condition is true, a block of code will be executed. in case of false, else block is executed
</td>
<td width="20%">
<code>let num = 5;
if(num = 4){
    console.log(true)
} else {
    console.log(false)
}
</code> <br/>
Output is false
</td>
</tr>

<tr>
<td width="20%">
if-else if-else
</td>
<td width="20%">
<code>if(<i>condition</i>){
    //Code Block...
} else if (<i>condition</i>) {
    //Code Block...
} else {
    //Code Block...
}
</code>
</td>
<td width="20%">
<b>else if</b> to specify a new condition to test, if the first/previous condition is false
</td>
<td width="20%">
<code>let num = 10;
if(num < 10){
    console.log("number is smaller");
} else if(num = 10) {
    console.log("number is equal");
} else {
    console.log("number is greater");
}
</code> <br/>
Output is number is equal
</td>
</td>
</tr>

<tr>
<td width="20%">
switch
</td>
<td width="20%">
<code>switch(expression) {
case &lt;value1&gt;:
    //code
    break;
case &lt;value2&gt;:
    //code
    break;
.
.
.
default:
    //default code block
}
</code>
</td>
<td width="20%">
<b>switch</b> to select one of many blocks of code to be executed. And <b>break</b> is used to end the preocessing within the switch statement.
</td>
<td width="20%">
<code>let num = 2;
switch(num) {
    case 1: console.log("Hello world!");
            break;
    case 2: console.log("Hi");
            break;
    default: console.log("this is default");
}
</code> <br/>
Output is Hi
</td>
</tr>

<tr>
<th colspan="4">Other useful operations</th>
</tr>

<tr>
<td width="20%">
typeof
</td>
<td width="20%">
<code>typeof(operand)
</code>
</td>
<td width="20%"><b> typeof</b> operator returns a string indicating the type of the unevaluated operand
</td>
<td width="20%"><code>
console.log(typeOf("Hello"))
</code>
Output is "string"
</td>
</tr>

<tr>
<td width="20%">
isNaN
</td>
<td width="20%">
<code> isNaN(operand)
</code>
</td>
<td width="20%"><b> isNaN</b> determines whether a value is anythying but a number or not. It returns false for a number 
</td>
<td width="20%"><code>
console.log(isNaN("Hello"))
</code>
Output is true
</td>
</tr>

<tr>
<td width="20%">
parseInt
</td>
<td width="20%">
<code>
parseInt(string, radix)
</code>
</td>
<td width="20%"> <b> parseInt</b> is a function that parses a string argument and returns an integer of the specified radix.(radix is a base)
</td>
<td width="20%">//0011 is 3 for binary, since binary only has 2  numbers 0, 1 the radix is 2<br/>
<code>console.log(parseInt("0011", 2));
//Default parseInt takes decimal system
console.log(parseInt("54"));</code>
<br/>
Output is 3 54
</td>
</tr>

<tr>
<td width="20%">
parseFloat
</td>
<td width="20%">
<code>parseFloat(string)
</code>
<td width="20%"> <b> parseFloat</b> is a function that parses a string argument and returns an float
</td>
<td width="20%">
<code>parseFloat("3.14")</code>
<br/>
Output is 3.14
</td>
</tr>

</table>

This cheatsheet covers the JS you will mostly use. To learn more commands you can go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference).

