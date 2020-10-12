# wb02ti4
4TI
<?php
$servername = "localhost";
$username = "username";
$password = "password";
$dbname = "myDB
$conn = new mysqli($servername, $username, $password, $dbname);
if ($conn->connect_error) {
  die("Connection failed: " . $conn->connect_error);
}

$sql = "SELECT id, firstname, lastname FROM MyGuests";
$result = $conn->query($sql);

if ($result->num_rows > 0) {
  while($row = $result->fetch_assoc()) {
    echo "id: " . $row["id"]. " - Name: " . $row["firstname"]. " " . $row["lastname"]. "<br>";
  }
} else {
  echo "0 results";
}
$conn->close();
?>
# Project title
 
This project simply solves `this` problem.
 
Simple code example 
 
```php
use My\Super\Library\Class;
 
$data = [[1, 3], [1, 4], [2, 4], [3, 1], [4, 1], [4, 2]];
 
$object = new Class(1, 2, 3)
$object->makeAwesome($data);
```
 
## Documentation
 
To find out how to use this library follow [Documentation](http://link-to-documentation).
 
## Installation
 
You can install it with Composer:
 
```
composer require vendor/project
```
 
## Features
 
* Can make this and this
* Helps with some other problew
* Is awesome
 
## Contribute
 
* Issue Tracker: github.com/vendor/project/issues
* Source Code: github.com/vendor/project
* Tests: phpunit
 
## License
 
This project is released under the MIT Licence. See the bundled LICENSE file for details.
 
## Author
 
John Doe
