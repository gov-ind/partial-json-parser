# partial-json-parser
Parse complete javascript objects from partial JSON strings.

# Description
Incomplete JSON strings will be parsed to its nearest complete object. 

Input: 
`{
  name: {
    first: 'ind',
    last: 'go`
    
Output:
`{
  name: {
    first: 'ind'
  }
}`

# Installation
From the CLI:

    npm install --save partial-json-parser
    
From javascript:

    var partialParse = require('partial-json-parser');
    var output = partialParse('"key": "value"');
    
Alternatively, you can directly use the script in the browser with a script tag.