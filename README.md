# web.github.io
<!DOCTYPE html>
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

        /* Colors and typography */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }

        /* Layout */
        header, nav, main, footer {
            margin-bottom: 20px;
        }

        header {
            background: url('header-image.jpg') no-repeat center center/cover;
            color: white;
            text-align: center;
            padding: 100px 20px;
        }

        header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 15px;
            justify-content: center;
            background-color: #333;
            padding: 10px 0;
        }

        nav a {
            text-decoration: none;
            color: white;
            font-weight: bold;
        }

        main {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        #about {
            background: url('about-image.jpg') no-repeat center center/cover;
            padding: 40px 20px;
            color: white;
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
        <h1>Facts Around Globe</h1>
        <p>Discover interesting facts about our world</p>
    </header>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
    <main>
        <section id="home">
            <h1>Welcome to Facts Around Globe</h1>
            <p>This is an example of a webpage following best practices in coding.</p>
        </section>
        <section id="about">
            <h2>About Us</h2>
            <p>Facts Around Globe is dedicated to sharing fascinating facts about different places, cultures, and events around the world. Our mission is to educate and entertain our audience with well-researched and engaging content.</p>
        </section>
        <section id="contact">
            <h2>Contact Us</h2>
            <p>If you have any questions or would like to reach out to us, please use the contact information below:</p>
            <p>Phone: +254796447965</p>
            <p>Email: <a href="mailto:rumsfelddonald1@gmail.com">rumsfelddonald1@gmail.com</a></p>
            <p>Twitter: <a href="https://twitter.com/factsaroundglobe" target="_blank">@factsaroundglobe</a></p>
            <form id="contact-form">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
                
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                
                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="4" required></textarea>
                
                <button type="submit">Submit</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Facts Around Globe</p>
    </footer>
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const form = document.getElementById('contact-form');
            
            form.addEventListener('submit', (event) => {
                event.preventDefault();
                const name = document.getElementById('name').value;
                const email = document.getElementById('email').value;
                const message = document.getElementById('message').value;
                
                if (validateEmail(email)) {
                    alert(`Thank you, ${name}! Your message has been sent.`);
                    form.reset();
                } else {
                    alert('Please enter a valid email address.');
                }
            });
        });

        function validateEmail(email) {
            const re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            return re.test(email);
        }
    </script>
</body>
</html>
