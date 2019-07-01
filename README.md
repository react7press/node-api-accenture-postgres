# Express NodeJs Basic RestApi CRUD with PostGreSQL for Accenture

Example basic CRUD Node Rest API with PostGreSQL. Please $ npm i and then to start express server $ node index.js

# PostGreSQL Schema
To start PostGreSQL => psql <br>
postgres=# \connect api<br>
psql (11.3, server 11.4)<br>
You are now connected to database "api" as user "yourmachine".<br>
api=# \list<br>
<p>
                                  <center>List of databases</center>
   Name    |   Owner   | Encoding |   Collate   |    Ctype    |   Access privileges   <br>
-----------+-----------+----------+-------------+-------------+-----------------------<br>
 Crocsluts | Crocsluts | UTF8     | en_US.UTF-8 | en_US.UTF-8 | <br>
 api       | accenture | UTF8     | en_US.UTF-8 | en_US.UTF-8 | <br>
 postgres  | postgres  | UTF8     | en_US.UTF-8 | en_US.UTF-8 | <br>
 template0 | postgres  | UTF8     | en_US.UTF-8 | en_US.UTF-8 | =c/postgres          +<br>
           |           |          |             |             | postgres=CTc/postgres<br>
 template1 | postgres  | UTF8     | en_US.UTF-8 | en_US.UTF-8 | =c/postgres          +<br>
           |           |          |             |             | postgres=CTc/postgres<br>
 testdb    | Crocsluts | UTF8     | en_US.UTF-8 | en_US.UTF-8 | <br>
(6 rows)<br>
<p>
# Express User Credentials
const db = require('./queries')<br>
const Pool = require('pg').Pool<br>
const pool = new Pool({<br>
  user: 'accenture',<br>
  host: 'localhost',<br>
  database: 'api',<br>
  password: 'password',<br>
  port: 5432,<br>
})<br>




MIT 1.0, see [LICENSE](LICENSE).
