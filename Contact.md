<?php
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    $name = $_POST["name"];
    $email = $_POST["email"];
    $message = $_POST["message"];

    if ($name && $email && $message) {
        echo "Thank you, $name! We received your message.";
    } else {
        echo "Please fill all fields.";
    }
}
?>
