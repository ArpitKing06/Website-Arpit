<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Welcome to my website! I provide information, services, and updates on a wide range of topics.">
    <title>All-in-One Website</title>
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4b400; /* Yellowish-orange background */
        }
        header {
            background: linear-gradient(135deg, #f4b400, #ff8800);
            color: #fff;
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        header h1 {
            font-size: 2.5rem;
            margin: 0;
            text-transform: uppercase;
            letter-spacing: 3px;
        }
        nav ul {
            list-style-type: none;
            padding: 0;
        }
        nav ul li {
            display: inline-block;
            margin: 0 15px;
        }
        nav ul li a {
            color: white;
            font-weight: bold;
            text-transform: uppercase;
            text-decoration: none;
            transition: color 0.3s;
        }
        nav ul li a:hover {
            color: #ffdd57;
        }
        .container {
            padding: 40px;
            text-align: center;
        }
        section {
            margin: 20px 0;
            padding: 40px;
            background-color: #fff;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        section:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.2);
        }
        section h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #f36c3d;
        }
        footer {
            background: linear-gradient(135deg, #f4b400, #ff8800);
            color: #fff;
            padding: 20px 0;
            text-align: center;
            margin-top: 30px;
            box-shadow: 0 -4px 6px rgba(0, 0, 0, 0.1);
        }
        form {
            display: flex;
            flex-direction: column;
            align-items: center;
            max-width: 600px;
            margin: auto;
        }
        input, textarea {
            width: 90%;
            max-width: 500px;
            padding: 15px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
        }
        button {
            padding: 15px 30px;
            background-color: #f36c3d;
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.2s;
        }
        button:hover {
            background-color: #ff8800;
            transform: scale(1.05);
        }
        #successMessage {
            display: none;
            margin-top: 20px;
            padding: 20px;
            background-color: #4CAF50;
            color: white;
            font-weight: bold;
            border-radius: 5px;
            animation: fadeIn 0.5s ease-in-out;
        }
        /* Animation for marquee */
        .marquee {
            font-size: 1.5rem;
            font-weight: bold;
            color: #46e34c;
            background-color: #333;
            padding: 15px 0;
        }
        /* Slow marquee with scroll amount */
        marquee {
            scrollamount: 2;
        }
        @keyframes fadeIn {
            0% { opacity: 0; }
            100% { opacity: 1; }
        }
        img {
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
            transition: transform 0.3s;
        }
        img:hover {
            transform: scale(1.05);
        }
    </style>
    <script>
        function validateForm() {
            const name = document.forms["contactForm"]["name"].value;
            const email = document.forms["contactForm"]["email"].value;
            const message = document.forms["contactForm"]["message"].value;
            
            if (name === "" || email === "" || message === "") {
                alert("Please fill out all fields.");
                return false;
            } else {
                showSuccessMessage();
                return false; // Prevent form submission
            }
        }

        function showSuccessMessage() {
            const successMessage = document.getElementById("successMessage");
            successMessage.style.display = "block";

            // Hide the success message after 0.5 minute (30,000 ms)
            setTimeout(function() {
                successMessage.style.display = "none";
            }, 30000); // 0.5 minute
        }
    </script>
</head>
<body>

<header>
    <h1>Welcome to My All-in-One Website</h1>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About Me</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#Logo">My logo</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

<!-- Marquee Section -->
<marquee class="marquee" behavior="scroll" direction="left">
    Welcome to the official website of Arpit Raj, also known as Arpit_King! Stay tuned for updates. Rock with us 🤘🏻
</marquee>

<div class="container">

    <!-- Home Section -->
    <section id="home">
        <h2>Home</h2>
        <p>Welcome to my website. I am Arpit Raj, also known as Arpit_King#3917. I am a <p>6<sup>th</sup></p> standard student. I live in Jaipur. Know more about me.</p>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Me</h2>
        <p>I am a regional level Basketball player. My hobbies are playing Basketball, Cricket, and reading books.</p>
    </section>

    <!-- Services Section -->
    <section id="services">
        <h2>Our Services</h2>
        <p>We provide various services including:</p>
        <ul>
            <li>Web Design</li>
            <li>Content Creation</li>
            <li>Logo Design</li>
            <li>Math expertise</li>
        </ul>
    </section>

    <!-- Logo Section -->
    <section id="Logo">
        <h2>My logo</h2>
        <p><img src="C:/Users/user/Desktop/Arpit Raj/New logo.jpg" alt="Arpit_King Logo" width="250" height="250"></p>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Us</h2>
        <div class="contact-container">
            <form name="contactForm" id="contactForm" onsubmit="return validateForm()">
                <input type="text" name="name" placeholder="Your Name" required>
                <input type="email" name="email" placeholder="Your Email" required>
                <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
                <button type="submit">Submit</button>
            </form>
            <div id="successMessage">Your message has been delivered to Arpit_King!</div>
        </div>
    </section>

</div>

<footer>
    <p>&copy; 2024 All-in-One Website. All Rights Reserved.</p>
    <p>Made by Arpit_King</p>
</footer>

</body>
</html>

 
