<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trinity Party Rentals</title>
    <style>
        body {
            font-family: sans-serif;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }

        header {
            background-color: #333;
            color: white;
            padding: 1rem 0;
            text-align: center;
        }

        nav {
            background-color: #444;
            color: white;
            text-align: center;
            padding: 0.5rem 0;
        }

        nav a {
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
        }

        nav a:hover {
            background-color: #555;
        }

        .container {
            width: 80%;
            margin: 2rem auto;
            overflow: auto;
        }

        .product {
            width: 30%;
            float: left;
            margin: 1rem;
            padding: 1rem;
            border: 1px solid #ddd;
            text-align: center;
        }

        .product img {
            max-width: 100%;
            height: auto;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1rem 0;
            position: relative;
            bottom: 0;
            width: 100%;
        }

        .contact-form {
          width:50%;
          margin: 2rem auto;
          padding: 1rem;
          border: 1px solid #ddd;
        }

        .contact-form label, .contact-form input, .contact-form textarea{
          display:block;
          margin-bottom: 0.5rem;
          width: 100%;
          box-sizing: border-box;
        }

        .contact-form button{
          background-color: #4CAF50; /* Green */
          border: none;
          color: white;
          padding: 15px 32px;
          text-align: center;
          text-decoration: none;
          display: inline-block;
          font-size: 16px;
        }

    </style>
</head>
<body>

    <header>
        <h1>Trinity Party Rentals</h1>
        <p>Your one-stop shop for all your party needs!</p>
    </header>

    <nav>
        <a href="#products">Products</a>
        <a href="#contact">Contact Us</a>
    </nav>

    <div class="container" id="products">
        <h2>Our Products</h2>

        <div class="product">
            <img src="placeholder_chair.jpg" alt="Chair">
            <h3>Chairs</h3>
            <p>Comfortable and stylish chairs for any event.</p>
        </div>

        <div class="product">
            <img src="placeholder_table.jpg" alt="Table">
            <h3>Tables</h3>
            <p>Various sizes and styles of tables available.</p>
        </div>

        <div class="product">
            <img src="placeholder_tent.jpg" alt="Tent">
            <h3>Tents</h3>
            <p>Protect your guests from the elements with our tents.</p>
        </div>

        <div class="product">
            <img src="placeholder_bouncehouse.jpg" alt="Bounce House">
            <h3>Bounce Houses</h3>
            <p>Fun for all ages! Bounce houses for your party needs.</p>
        </div>

        <div class="product">
            <img src="placeholder_linens.jpg" alt="Linens">
            <h3>Linens</h3>
            <p>Various colors and styles to match your theme.</p>
        </div>
        <div class="product">
            <img src="placeholder_decorations.jpg" alt="Decorations">
            <h3>Decorations</h3>
            <p>Make your party amazing with our decorations.</p>
        </div>
        </div>

    <div class="container" id="contact">
      <h2>Contact Us</h2>
      <div class="contact-form">
        <form id="contactForm">
          <label for="name">Name:</label>
          <input type="text" id="name" name="name" required>

          <label for="email">Email:</label>
          <input type="email" id="email" name="email" required>

          <label for="message">Message:</label>
          <textarea id="message" name="message" rows="4" required></textarea>

          <button type="submit">Submit</button>
        </form>
      </div>

    </div>

    <footer>
        <p>&copy; 2024 Trinity Party Rentals</p>
    </footer>
    <script>
      document.getElementById('contactForm').addEventListener('submit', function(event) {
        event.preventDefault(); // Prevent default form submission
        // Here you would add code to handle form submission, like sending an email.
        // For now, just logging the form data:
        const formData = new FormData(event.target);
        const formValues = {};
        formData.forEach((value, key) => formValues[key] = value);
        console.log(formValues);
        alert("Form Submitted! (Check console for data)"); // Simple feedback
      });
    </script>

</body>
</html>
