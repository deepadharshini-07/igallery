# Ex.08 Design of Interactive Image Gallery
## Date:15:12:2024

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
home.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home</title>
    <style>
        body { 
            font-family: Arial, sans-serif; 
            margin: 0; 
            background-image: url('Hogwards.png'); 
            background-size: cover; 
            background-repeat: no-repeat; 
            background-attachment: fixed; 
        }
        header { 
            background: rgba(0, 0, 0, 0.7); 
            color: white; 
            padding: 10px; 
            text-align: center; 
        }
        nav a { 
            color: white; 
            margin: 0 15px; 
            text-decoration: none; 
        }
        nav a:hover { 
            text-decoration: underline; 
        }
        main { 
            text-align: center; 
            padding: 20px; 
            background: rgba(255, 255, 255, 0.8); 
            margin: 50px auto;
            max-width: 600px;
            border-radius: 10px;
        }
        footer { 
            background: rgba(0, 0, 0, 0.7); 
            color: white; 
            text-align: center; 
            padding: 10px; 
            position: relative; 
            bottom: 0; 
            width: 100%; 
        }
        footer p { 
            margin: 5px 0; 
        }
        footer a { 
            color: lightblue; 
            text-decoration: none; 
        }
        footer a:hover { 
            text-decoration: underline; 
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="gallery.html">Gallery</a>
            <a href="about.html">About Us</a>
            <a href="contact.html">Contact Us</a>
        </nav>
    </header>
    <main>
        <h1>Welcome to Our Image Gallery</h1>
        <p>Explore the world with us through images.</p>
    </main>
    <footer>
        <p>&copy; 2024 Designed and Developed by DEEPADHARSHINI T</p>
            </footer>
</body>
</html>

gallery.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }
        header {
            background: #333;
            color: white;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }
        nav a:hover {
            text-decoration: underline;
        }
        main {
            flex: 1; /* Ensures main content stretches to push footer to the bottom */
            padding: 20px;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
            padding: 20px;
        }
        .photo {
            background: white;
            border: 1px solid #ddd;
            border-radius: 10px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            width: 250px;
            text-align: center;
        }
        .photo img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .photo-title {
            font-size: 18px;
            font-weight: bold;
            margin: 10px 0;
        }
        .photo-description {
            font-size: 14px;
            color: #555;
            margin: 0 10px 10px;
        }
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 10px;
            width: 100%;
        }
        footer a {
            color: lightblue;
            text-decoration: none;
            margin: 0 5px;
        }
        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="gallery.html">Gallery</a>
            <a href="about.html">About Us</a>
            <a href="contact.html">Contact Us</a>
        </nav>
    </header>
    <main>
        <h1 style="text-align: center; margin: 20px 0;">Photo Gallery</h1>
        <div class="gallery">
                <div class="photo">
                <img src="Car.png" alt="Car">
                <p>Car</p>
                </div>
                <div class="photo">
                <img src="Harry Potter.png" alt="Harry Potter">
                <p>Harry Potter</p>
                </div>
                <div class="photo">
                <img src="Stadium.png" alt="Stadium">
                <p>Stadium</p>
                </div>
                <div class="photo">
                <img src="Music.png" alt="Music">
                <p>Music</p>
                </div>
                <div class="photo">
                <img src="Cinema.png" alt="Cinmea">
                <p>Cinema</p>
                </div>
                <div class="photo">
                <img src="Plane.png" alt="Plane">
                <p>Plane</p>
                </div>
                <div class="photo">
                <img src="Wizards.png" alt="Wizards">
                <p>Wizards</p>
                </div>

                        </div>
    </main>
    <footer>
       <p> &copy; 2024 Designed and Developed by DEEPADHARSHINI T</p>
    </footer>
</body>
</html>

about.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }
        header {
            background: #333;
            color: white;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }
        nav a:hover {
            text-decoration: underline;
        }
        main {
            flex: 1; /* Ensures main content stretches to push footer to the bottom */
            padding: 20px;
            text-align: center;
        }
        main .content {
            max-width: 600px;
            margin: 0 auto;
            text-align: left;
        }
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 10px;
            width: 100%;
        }
        footer a {
            color: lightblue;
            text-decoration: none;
            margin: 0 5px;
        }
        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="gallery.html">Gallery</a>
            <a href="about.html">About Us</a>
            <a href="contact.html">Contact Us</a>
        </nav>
    </header>
    <main>
        <h1>About Us</h1>
        <div class="content">
            <p>Welcome to Image Gallery, where we showcase stunning images from around the world.Explore the world through our pictures</p> 
            <p>Founded in 2024,Images and media are powerful communication devices. They are useful for conveying concepts and information, and they can help improve comprehension by reinforcing information provided in text. But images and media attract and engage our attention.</p>
            <p>Thank you for visiting, and we hope you enjoy our gallery!</p>
        </div>
    </main>
    <footer>
        <p>&copy; 2024 Designed and Developed by DEEPADHARSHINI T</p>
    </footer>
</body>
</html>

contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }
        header {
            background: #333;
            color: white;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }
        nav a:hover {
            text-decoration: underline;
        }
        main {
            flex: 1; 
            padding: 20px;
            text-align: center;
        }
        main form {
            max-width: 500px;
            margin: 0 auto;
            text-align: left;
        }
        form label {
            display: block;
            margin-top: 10px;
            font-weight: bold;
        }
        form input, form textarea {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 14px;
        }
        form button {
            margin-top: 15px;
            padding: 10px 20px;
            background: #333;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        form button:hover {
            background: #555;
        }
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 10px;
            width: 100%;
        }
        footer a {
            color: lightblue;
            text-decoration: none;
            margin: 0 5px;
        }
        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="gallery.html">Gallery</a>
            <a href="about.html">About Us</a>
            <a href="contact.html">Contact Us</a>
        </nav>
    </header>
    <main>
        <h1>Contact Us</h1>
        <section class="contact">
        <h2>Get in Touch</h2>
        <p><strong>Website Handeled By:</strong> Deepadharshini T</p>
        <p><strong>Phone:</strong> 9876543210</p>
        <p><strong>Email:</strong> imagegallery@gmail.com</p>
    </section>

            </main>
    <footer>
        <p>&copy; 2024  Designed and Developed by DEEPADHARSHINI T</p>  
 </footer>
</body>
</html>

```
## OUTPUT:
![alt text](<Screenshot 2024-12-15 154945.png>)

![alt text](<Screenshot 2024-12-15 154957.png>)

![alt text](<Screenshot 2024-12-15 155010.png>)

![alt text](<Screenshot 2024-12-15 155023.png>)




## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
