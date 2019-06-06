# Blog written by Alex Baban

## Some sample JavaScript

```js

// using https://www.npmjs.com/package/mysql
const mysql = require('mysql');

const connection = mysql.createConnection(
    {
        host: 'some.domain.com',
        user: 'someuser',
        password: 'somepassword',
        database: 'somedb'
    });

connection.connect(
    function (err) {
        if (err) throw err;
        console.log('Connected!');
    });

connection.query(
    'SELECT * FROM users',
    function (err, rows) {
        if (err) throw err;
        console.log(rows);
    });

connection.end(
    function (err) {
        // connection is terminated gracefully
    });
    
 ```
 
Foo bar baz.  
 
## Something something
 
hey, hey, hey
