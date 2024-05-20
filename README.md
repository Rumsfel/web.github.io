# web.github.io
DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Facts Around Globe</title>
    <style>
        /* Basic reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Typography */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            padding: 20px;
            background-color: #f9f9f9;
        }

        /* Layout */
        header, nav, main, footer {
            margin-bottom: 20px;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 15px;
            justify-content: center;
        }

        nav a {
            text-decoration: none;
            color: #333;
        }

        h1, h2 {
            margin-bottom: 10px;
        }

        main {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        form label {
            display: block;
            margin-bottom: 5px;
        }

        form input, form textarea {
            margin-bottom: 10px;
            padding: 8px;
            width: 100%;
            max-width: 300px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            padding: 10px 15px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }

        footer {
            text-align: center;
            padding: 10px;
            background: #333;
            color: white;
        }

        footer p {
            margin: 5px 0;
        }

        /* Responsive design */
        @media (max-width: 600px) {
            nav ul {
                flex-direction: column;
                align-items: center;
            }

            form input, form textarea {
                width: 100%;
            }

            main {
                padding: 10px;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="home">
            <h1>Facts Around Globe</h1>
            <p>Welcome to Facts Around Globe. Discover interesting facts about our world.</p>
        </section>
        <section id="about">
            <h2>About Us</h2>
            <p>Facts Around Globe is dedicated to sharing fascinating facts about different places, cultures, and events around the world. Our mission is to educate and entertain our audience with well-researched and engaging content.</p>
        </section>
        <section id="contact">
            <h2>Contact Us</h2>
            <p>If you have any questions or would like to reach out to us, please use the contact information below:</p>
            <p>Phone: +254796447965</p>
            <p>Twitter: <a href="https://twitter.com/factsaroundglobe" target="_blank">@factsaroundglobe</a></p>
            <form id="contact-form">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
                
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                
                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="4" required></texta…
