<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Header</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="logo">
            <h1>My Website</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
        <div class="header-buttons">
            <a href="#login" class="button">Login</a>
            <a href="#signup" class="button">Sign Up</a>
        </div>
    </header>
</body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background-color: #333;
    color: #fff;
}

.logo h1 {
    font-size: 24px;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

nav ul li a {
    text-decoration: none;
    color: #fff;
    padding: 8px 16px;
    border-radius: 4px;
    transition: background-color 0.3s ease;
}

nav ul li a:hover {
    background-color: #555;
}

.header-buttons .button {
    text-decoration: none;
    color: #fff;
    padding: 10px 20px;
    border-radius: 4px;
    background-color: #007BFF;
    margin-left: 10px;
    transition: background-color 0.3s ease;
}

.header-buttons .button:hover {
    background-color: #0056b3;
}

@media (max-width: 768px) {
    header {
        flex-direction: column;
        text-align: center;
    }

    nav ul {
        flex-direction: column;
        gap: 10px;
    }

    .header-buttons {
        margin-top: 10px;
    }
}
