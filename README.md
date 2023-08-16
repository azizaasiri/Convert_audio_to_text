# Convert audio to text

To receive the text from the request , used this code:
```
$text = $_POST['text'];
```

To connect to the database and save the text :
```

$servername = "localhost";
$username = "rooot";
$password = "root";
$dbname = "voice";

```

To establish the connection to the database:
```
$conn = new mysqli("localhost", "rooot", "root", "voice");

```

Execute a query to save the text in the database:
```
$sql = "INSERT INTO texts (text) VALUES ('$text')";
```

To close the connection to the database:
```
$conn->close();
```
