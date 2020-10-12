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
# Tytuł projektu
 
This project simply solves `this` problem.
 
Simple code example 
 
```php
use My\Super\Library\Class;
 
$data = [[1, 3], [1, 4], [2, 4], [3, 1], [4, 1], [4, 2]];
 
$object = new Class(1, 2, 3)
$object->makeAwesome($data);
```
 
## Dokumentacja
 
Moja dokumentacja dotycząca pracy w domu na zajęciach tworzenie i aplikacji
 
## Instalacja
 
Instalacja została wykonana na zajęciach.

Możesz zainstalowac to z kompozytorium
 
```
https://github.com/BOJANNNN/wb02ti4
```
 
## Cel i Funkcje
 
 * Zbiór elementów pracy w domu
 * Możliwość pomocy kolegów z zaspołu projektowego
 * Nadzór kierownika projektu
 
## Wkład projektowy
 
* Główny nadzór: https://github.com/BOJANNNN
* Kod projektu:  https://github.com/BOJANNNN
 
## Licencja
 Ten projekt jest udostępniany na licencji MIT. Szczegółowe informacje można znaleźć w dołączonym pliku LICENCJA.
 
## Autor
 
Wiktor Bojanowski
