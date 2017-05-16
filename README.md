# linebyline
A Node.js module for reading file line by line synochronicaly   

## Examples
<pre>
const LineByLine = require('./readlinesyn');   
  
var filename = './result.txt';  
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
