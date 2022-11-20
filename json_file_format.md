`JSON (Java Script Object Notation)` is a text-based data exchange format. JSON is a good alternative to XML. </br>
JSON is derived from `JavaScript` but is language independent data format. </br>




It is a collection of key-value pairs where the key must be a string type, and the value can be of any of the following types:
- Number 
- String 
- Boolean
- Array 
- Object
- null



A couple of important rules to note:

- In the JSON data format, the keys must be enclosed in double quotes.
- The key and value must be separated by a colon (:) symbol.
- There can be multiple key-value pairs. Two key-value pairs must be separated by a comma (,) symbol.
- No comments (// or /* */) are allowed in JSON data. Meaning you can't add comments. But you still can which we'll see later.



Here is how some simple JSON data looks:
```json
{
    "name": "Alex C",
    "age": 2,
    "city": "Houston"
}
```

Valid JSON data can be in two different formats:
- A collection of key-value pairs enclosed by a pair of curly braces {...}. Ex:- The above example
- A collection of an ordered list of key-value pairs seperated by comma and enclosed by a pair of square brackets [....]. 
Example:- 
```
[
	{
        "name": "Alex C",
        "age": 2,
        "city": "Houston"
	},
    {
        "name": "Jack G",
        "age": 56,
        "city": "Washington"
	},
   
]
```


If you are a JavaScript developer, you might feel that JSON format and JavaScript objects are very similar. But actually, they are not.   
The structure of the JSON format was derived from the JavaScript object syntax. That's the only relationship between the JSON data format and JavaScript objects.
JSON is a programming language-independent format. We can use the JSON data format in Python, Java, PHP, and many other programming languages. 
You can save JSON data in a file with an extension of `.json` . 
