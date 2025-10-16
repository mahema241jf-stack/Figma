# Ex09 Event Registration Web Application
## Date:16/10/2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
project.html
project.html


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble Clone</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        /* Ensuring that all images have consistent dimensions */
        .card-img-top {
            width: 100%;
            height: 250px; /* Adjust the height to maintain consistent size */
            object-fit: cover; /* Ensures that the image covers the area without stretching */
        }
        footer {
            background-color: #f8f9fa;
            padding: 20px 0;
            text-align: center;
            width: 100%;
            bottom: 0px;
        }
    </style>
</head>
<body>
    {% load static %}

    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container">
            <a class="navbar-brand" href="#">
                <img src="{% static 'images/logo.png' %}" alt="Dribbble Clone Logo" height="40">
            </a>

            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#features">Features</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#portfolio">Portfolio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#contact">Contact</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link btn btn-primary text-white" href="{% url 'signup' %}">Sign Up</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    <header class="bg-primary text-white text-center py-5">
        <div class="container">
            <h1>Show Your Creativity to the World</h1>
            <p class="lead">Join the platform where designers share, grow, and inspire.</p>
            <a href="#portfolio" class="btn btn-light btn-lg">Get Started</a>
        </div>
    </header>
    <section id="features" class="py-5">
        <div class="container">
            <h2 class="text-center mb-4">Features</h2>
            <div class="row text-center">
                <div class="col-md-4">
                    <div class="card shadow-sm">
                        <div class="card-body">
                            <h5 class="card-title">For Designers</h5>
                            <p class="card-text">Showcase your portfolio and gain exposure to potential clients. Build your brand and get noticed by top businesses and teams.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card shadow-sm">
                        <div class="card-body">
                            <h5 class="card-title">For Inspiration</h5>
                            <p class="card-text">Discover creative ideas from a global community of designers. Get inspired by the latest trends and innovative designs from industry experts.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card shadow-sm">
                        <div class="card-body">
                            <h5 class="card-title">For Businesses</h5>
                            <p class="card-text">Connect with top designers to bring your ideas to life. Find the right creative talent to help you design and build your brand’s future.</p>
                        </div>
                    </div>
                </div>                
            </div>
        </div>
    </section>
    <section id="portfolio" class="py-5 bg-light">
        <div class="container">
            <h2 class="text-center mb-4">Portfolio</h2>
            <p class="text-center mb-4">Explore some of the best creative works shared by the community.</p>
            <div class="row">
                <!-- Portfolio items here... -->
                <div class="col-md-4 mb-4">
                    <div class="card">
                        <img src="{% static 'images/retro.png' %}" class="card-img-top" alt="Retrospective Branding Design">
                        <div class="card-body">
                            <h5 class="card-title">Retrospective Branding Design</h5>
                            <p class="card-text">A modern take on retro branding elements, blending classic typography with contemporary aesthetics.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="card">
                        <img src="{% static 'images/house.png' %}" class="card-img-top" alt="Home Swap Platform UI Elements">
                        <div class="card-body">
                            <h5 class="card-title">Home Swap Platform UI Elements</h5>
                            <p class="card-text">UI design for a home exchange platform, featuring intuitive navigation and user-friendly interfaces.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="card">
                        <img src="{% static 'images/jewel.png' %}" class="card-img-top" alt="Jewelry Website Design">
                        <div class="card-body">
                            <h5 class="card-title">Jewelry Website Design</h5>
                            <p class="card-text">An elegant e-commerce website design for a jewelry brand, emphasizing luxury and user experience.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="card">
                        <img src="{% static 'images/ev.png' %}" class="card-img-top" alt="EV Charging Station Branding">
                        <div class="card-body">
                            <h5 class="card-title">EV Charging Station Branding</h5>
                            <p class="card-text">Brand identity design for an electric vehicle charging station, incorporating eco-friendly themes.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="card">
                        <img src="{% static 'images/fitness.png' %}" class="card-img-top" alt="Fitness App UI Design">
                        <div class="card-body">
                            <h5 class="card-title">Fitness App UI Design</h5>
                            <p class="card-text">A sleek and modern user interface design for a fitness tracking mobile application.</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 mb-4">
                    <div class="card">
                        <img src="{% static 'images/coffee.png' %}" class="card-img-top" alt="Coffee Shop Logo Design">
                        <div class="card-body">
                            <h5 class="card-title">Coffee Shop Logo Design</h5>
                            <p class="card-text">A minimalist and cozy logo design for a local coffee shop, capturing the essence of warmth.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section id="contact" class="py-5">
        <div class="container contact-container">
            <h2 class="text-center mb-4">Contact Us</h2>
            <p class="text-center mb-4">We'd love to hear from you. Whether you have a question, feedback, or suggestion, feel free to reach out to us using the form below.</p>
            <form action="#" method="POST">
                <div class="mb-3">
                    <label for="name" class="form-label">Full Name</label>
                    <input type="text" class="form-control" id="name" name="name" required>
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Email address</label>
                    <input type="email" class="form-control" id="email" name="email" required>
                </div>
                <div class="mb-3">
                    <label for="subject" class="form-label">Subject</label>
                    <input type="text" class="form-control" id="subject" name="subject" required>
                </div>
                <div class="mb-3">
                    <label for="message" class="form-label">Message</label>
                    <textarea class="form-control" id="message" name="message" rows="4" required></textarea>
                </div>
                <button type="submit" class="btn btn-primary w-100">Send Message</button>
            </form>
        </div>
    </section>
    <footer>
        <p>&copy; 2025  All rights reserved.</p>
    </footer>
</body>
</html>

signup.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign Up - Dribbble Clone</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        .container {
            max-width: 500px;
        }
        .form-container {
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            background-color: #fff;
        }
    </style>
</head>
<body>
    <div class="container mt-5">
        <div class="form-container">
            <h2 class="text-center mb-4">Create an Account</h2>
            <form action="#" method="POST">
                <div class="mb-3">
                    <label for="fullName" class="form-label">Full Name</label>
                    <input type="text" class="form-control" id="fullName" name="fullName" required>
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Email address</label>
                    <input type="email" class="form-control" id="email" name="email" required>
                </div>
                <div class="mb-3">
                    <label for="password" class="form-label">Password</label>
                    <input type="password" class="form-control" id="password" name="password" required>
                </div>
                <div class="mb-3">
                    <label for="confirmPassword" class="form-label">Confirm Password</label>
                    <input type="password" class="form-control" id="confirmPassword" name="confirmPassword" required>
                </div>
                <div class="mb-3 form-check">
                    <input type="checkbox" class="form-check-input" id="terms" required>
                    <label class="form-check-label" for="terms">I agree to the terms and conditions</label>
                </div>
                <button type="submit" class="btn btn-primary w-100">Sign Up</button>
            </form>
            <p class="text-center mt-3">Already have an account? <a href="login.html">Login here</a></p>
        </div>
    </div>
</body>
</html>

views.py
from django.shortcuts import render
def home_view(request):
    return render(request, 'project.html')
def signup(request):
    return render(request, 'signup.html')


```

## OUTPUT:

<img width="1700" height="734" alt="Screenshot (71)" src="https://github.com/user-attachments/assets/c778efb4-b6c0-420d-b36e-406aea6ce28c" />


<img width="1920" height="1080" alt="Screenshot (72)" src="https://github.com/user-attachments/assets/795ceb4f-8fae-4ea9-bc79-5203793a132d" />
<img width="1015" height="469" alt="Screenshot (79)" src="https://github.com/user-attachments/assets/5a75b3e0-25c8-4a55-82fb-dcf4a4e10b5c" />
<img width="1009" height="502" alt="Screenshot (80)" src="https://github.com/user-attachments/assets/ce6d2c4a-75da-4078-a117-4870d159570b" />


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
