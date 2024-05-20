# web.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Best Practices Webpage</title>
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
        }

        /* Layout */
        header, nav, main, footer {
            margin-bottom: 20px;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 15px;
        }

        nav a {
            text-decoration: none;
            color: #333;
        }

        h1, h2 {
            margin-bottom: 10px;
        }

        form label {
            display: block;
            margin-bottom: 5px;
        }

        form input {
            margin-bottom: 10px;
            padding: 8px;
            width: 100%;
            max-width: 300px;
        }

        /* Responsive design */
        @media (max-width: 600px) {
            nav ul {
                flex-direction: column;
            }

            form input {
                width: 100%;
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
            <h1>Welcome to Our Website</h1>
            <p>This is an example of a webpage following best practices in coding.</p>
        </section>
        <section id="about">
            <h2>About Us</h2>
            <p>Information about our company.</p>
        </section>
        <section id="contact">
            <h2>Contact Us</h2>
            <form id="contact-form" action="/submit-form" method="post">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
                
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                
                <button type="submit">Submit</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Best Practices Webpage</p>
    </footer>
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const form = document.getElementById('contact-form');
            
            form.addEventListener('submit', (event) => {
                event.preventDefault();
                const name = document.getElementById('name').value;
                const email = document.getElementById('email').value;
                
                if (validateEmail(email)) {
                    alert(`Thank you, ${name}! Your form has been submitted.`);
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
