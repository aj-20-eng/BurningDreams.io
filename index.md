<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Burning Dreams Portfolio</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
            color: #333;
        }
        header {
            background-color: #ff4500;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
        }
        nav a {
            color: #fff;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
        }
        nav a:hover {
            background-color: #ddd;
            color: black;
        }
        .content {
            padding: 20px;
        }
        .links a {
            display: block;
            margin: 10px 0;
            padding: 10px;
            background-color: #ff4500;
            color: #fff;
            text-decoration: none;
            text-align: center;
        }
        .links a:hover {
            background-color: #333;
        }
        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 20px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Burning Dreams</h1>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
    </nav>
    <div class="content" id="home">
        <h2>Welcome to Burning Dreams</h2>
        <p>We are a passionate team dedicated to making your dreams come true.</p>
        <div class="links">
            <a href="https://www.linkedin.com" target="_blank">LinkedIn</a>
            <a href="https://www.youtube.com" target="_blank">YouTube</a>
            <a href="https://www.telegram.com" target="_blank">Telegram</a>
        </div>
    </div>
    <div class="content" id="about" style="display:none;">
        <h2>About Us</h2>
        <p>Burning Dreams is a team of creative individuals who are dedicated to bringing your ideas to life. Our mission is to provide top-notch services to our clients and help them achieve their goals.</p>
    </div>
    <footer>
        <p>&copy; 2025 Burning Dreams. All Rights Reserved.</p>
    </footer>
    <script>
        document.querySelectorAll('nav a').forEach(link => {
            link.addEventListener('click', function() {
                document.querySelectorAll('.content').forEach(div => {
                    div.style.display = 'none';
                });
                document.querySelector(this.getAttribute('href')).style.display = 'block';
            });
        });
    </script>
</body>
</html>
