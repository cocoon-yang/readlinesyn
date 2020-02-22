# readlinesyn
A Node.js module for reading file line by line synochronicaly   


# Methods
  - open( filePath ) 
  - close()
  - next()
  - isEOF()

# Installation

readlinesyn requires [Node.js](https://nodejs.org/) v4+ to run.

```
$ npm install readlinesyn
```  


## Examples
<pre>
const LineByLine = require('./readlinesyn');   
  
var filename = './result.txt';  
// the default encode is 'utf8'
// liner._encode = "utf8";
var liner = new LineByLine();  
  
liner.open( filename );   
var theline;  
while( !liner.EOF() )  
{  
  theline = liner.next();  
   console.log( 'READ LINE: ' + theline );  
}  
  
liner.close();  
<pre>
