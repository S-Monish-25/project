# Project Responsive Web Design using Bootstrap
# Date:07/12/2024
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Design Portfolio</title>
    <link rel="stylesheet" href="dribble.css">
    <script>const searchBar = document.querySelector('.search-bar');

        searchBar.addEventListener('keydown', function(event) {
            if (event.key === 'Enter') {
                event.preventDefault(); // Prevent default form submission
                alert(Searching for: ${searchBar.value});
            }
        });</script>
        <style>
            body, h1, h2, p, a, input, button {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif; 
}

body {
    background-color: #f5f5f5;
    color: #333;
}

/* Top Bar Styling */
.top-bar {
    display: flex;
    align-items: center;
    background-color: #ffffff;
    padding: 10px 20px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.search-bar {
    margin-right: 15px;
    padding: 8px;
    border: 1px solid #ddd;
    border-radius: 4px;
    outline: none;
}

.nav-item {
    margin: 0 10px;
    color: #333;
    text-decoration: none;
}

.blue-text {
    color: #007bff;
    font-weight: bold;
}

.blue-text:hover {
    text-decoration: underline;
}

/* Header Section */
header {
    background-image: url('https://images.pexels.com/photos/1072179/pexels-photo-1072179.jpeg'); /* Add your header image */
    background-size: cover;
    padding: 80px 20px;
    text-align: center;
    color: #fff;
}

.header-content h1 {
    font-size: 36px;
    margin-bottom: 10px;
}

.header-content p {
    font-size: 18px;
    margin-bottom: 20px;
}

.search-input {
    padding: 10px;
    width: 60%;
    max-width: 500px;
    border: none;
    border-radius: 4px;
    outline: none;
}

/* Trending Searches Section */
.trending {
    padding: 20px;
    text-align: center;
}

.trending h2 {
    font-size: 24px;
    margin-bottom: 10px;
}

.trending-tags {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.trending-tags span {
    background-color: #007bff;
    color: #fff;
    padding: 5px 10px;
    margin: 5px;
    border-radius: 4px;
    font-size: 14px;
}

/* Gallery Section */
.gallery {
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
    width: 200px;
    text-align: center;
}

.card img {
    width: 100%;
    height: auto;
}

.card h3 {
    font-size: 16px;
    margin: 10px 0;
}

.card p {
    font-size: 12px;
    color: #555;
    margin-bottom: 10px;
}

/* Gallery Section */
.gallery {
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
    width: 200px;
    text-align: center;
    position: relative;
}

.card img {
    width: 100%;
    height: auto;
    transition: transform 0.3s ease;
}

.card:hover img {
    transform: scale(1.2); /* Scale image to 120% on hover */
}

.card h3 {
    font-size: 16px;
    margin: 10px 0;
}

.card p {
    font-size: 12px;
    color: #555;
    margin-bottom: 10px;
}

/* Footer Section */
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px 20px;
    margin-top: 20px;
}
        </style>
</head>
<body>
    <div class="top-bar">
        <input type="text" class="search-bar" placeholder="Search...">
        <a href="#" class="nav-item">Explore</a>
        <a href="#" class="nav-item">Hire a Designer</a>
        <a href="#" class="nav-item">Find Jobs</a>
        <a href="#" class="nav-item">Blog</a>
        <a href="signup.html" class="nav-item blue-text">Sign up</a>
        <a href="login.html" class="nav-item blue-text">Log in</a>
    </div>

    <!-- Header Section -->
    <header>
        <div class="header-content">
            <h1>Discover the world’s top designers</h1>
            <p>Explore work from the most talented and accomplished designers ready to take on your next project</p>
            <input type="text" class="search-input" placeholder="What are you looking for?">
        </div>
    </header>

    <!-- Trending Searches Section -->
    <section class="trending">
        <h2>Trending Searches</h2>
        <div class="trending-tags">
            <span>landing page</span>
            <span>e-commerce</span>
            <span>mobile app</span>
            <span>logo design</span>
            <span>dashboard</span>
            <span>icons</span>
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="gallery">

        <div class="card">
            <img src="1.jpg" alt="Design Sample">
            <h3>vijay</h3>
            
        </div>

        <div class="card">
            <img src="2.jpg" alt="Design Sample">
            <h3>surya</h3>
           
        </div>

        <div class="card">
            <img src="3.jpg" alt="Design Sample">
            <h3>ajith</h3>
            
        </div>

        <div class="card">
            <img src="4.jpg" alt="Design Sample">
            <h3>karthi</h3>
            
        </div>

        <div class="card">
            <img src="5.jpg" alt="Design Sample">
            <h3>vishal</h3>
        </div>

        <div class="card">
            <img src="6.jpg" alt="Design Sample">
            <h3>aravind</h3>
            
        </div>

        <div class="card">
            <img src="7.jpg" alt="Design Sample">
            <h3>dhoni</h3>
         
        </div>

        <div class="card">
            <img src="8.jpg" alt="Design Sample">
            <h3>virat</h3>
            
        </div>

        <div class="card">
            <img src="9.jpg" alt="Design Sample">
            <h3>sachin</h3>
          
        </div>

        <div class="card">
            <img src="10.jpg" alt="Design Sample">
            <h3>mitchell</h3>
          
        </div>

        <div class="card">
            <img src="11.jpg" alt="Design Sample">
            <h3>raina</h3>
          
        </div>

        <div class="card">
            <img src="12.jpg" alt="Design Sample">
            <h3>jadeja</h3>
            
        </div>
        <!-- Add more cards as needed -->
    </section>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2024 Design Portfolio. All rights reserved.</p>
    </footer>

    <script src="dribble.js"></script>
</body>
</html>
```
```
login
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Login Page</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background:rgb(58, 182, 227);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: #fff;
        }
        .card {
            border-radius: 20px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            background: #fff;
            color: #000;
        }
        .card-header {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
            text-align: center;
            font-size: 1.5rem;
            font-weight: bold;
            color:cornflowerblue;
            background: #f8f9fa;
            border-top-left-radius: 20px;
            border-top-right-radius: 20px;
        }
        .card-header img {
            width: 30px;
            height: 30px;
        }
        .btn-primary {
            background-color: #000;
            border: none;
            color: #fff;
        }
        .btn-primary:hover {
            background-color: #333;
        }
        .form-control:focus {
            box-shadow: none;
            border-color: #000;
        }
        .link:hover {
            text-decoration: underline;
            color: #000;
        }
        .text-center a {
            color: #000;
        }
        .text-center a:hover {
            text-decoration: underline;
            color: #000;
        }
    </style>
</head>
<body>
    <div class="card p-4" style="width: 22rem;">
        <div class="card-header">
            Login
        </div>
        <div class="card-body">
            <form>
                <div class="mb-3">
                    <label for="email" class="form-label">Email address</label>
                    <input type="email" class="form-control" id="email" placeholder="Enter your email" required>
                </div>
                <div class="mb-3">
                    <label for="password" class="form-label">Password</label>
                    <input type="password" class="form-control" id="password" placeholder="Enter your password" required>
                </div>
                <div class="d-flex justify-content-between align-items-center">
                    <div>
                        <input type="checkbox" id="rememberMe">
                        <label for="rememberMe" class="form-label">Remember me</label>
                    </div>
                    <a href="#" class="text-decoration-none link">Forgot Password?</a>
                </div>
                <button type="submit" class="btn btn-primary w-100 mt-3">Login</button>
            </form>
        </div>
        <div class="text-center mt-3">
            <span>Don't have an account? <a href="signup.html" target="_blank" class="text-decoration-none link">Sign Up</a></span>
        </div>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```
```
sign up
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Sign Up Page</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background:rgb(95, 212, 208);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: #fff;
        }
        .card {
            border-radius: 20px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            background: #fff;
            color: #000;
        }
        .card-header {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
            text-align: center;
            font-size: 1.5rem;
            font-weight: bold;
            color:cornflowerblue;
            background: #f8f9fa;
            border-top-left-radius: 20px;
            border-top-right-radius: 20px;
        }
        .card-header img {
            width: 30px;
            height: 30px;
        }
        .btn-primary {
            background-color: #000;
            border: none;
            color: #fff;
        }
        .btn-primary:hover {
            background-color: #333;
        }
        .form-control:focus {
            box-shadow: none;
            border-color: #000;
        }
        .link:hover {
            text-decoration: underline;
            color: #000;
        }
        .text-center a {
            color: #000;
        }
        .text-center a:hover {
            text-decoration: underline;
            color: #000;
        }
    </style>
</head>
<body>
    <div class="card p-4" style="width: 22rem;">
        <div class="card-header">
            Sign Up
        </div>
        <div class="card-body">
            <form>
                <div class="mb-3">
                    <label for="fullName" class="form-label">Full Name</label>
                    <input type="text" class="form-control" id="fullName" placeholder="Enter your full name" required>
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Email address</label>
                    <input type="email" class="form-control" id="email" placeholder="Enter your email" required>
                </div>
                <div class="mb-3">
                    <label for="password" class="form-label">Password</label>
                    <input type="password" class="form-control" id="password" placeholder="Enter your password" required>
                </div>
                <div class="mb-3">
                    <label for="confirmPassword" class="form-label">Confirm Password</label>
                    <input type="password" class="form-control" id="confirmPassword" placeholder="Confirm your password" required>
                </div>
                <button type="submit" class="btn btn-primary w-100 mt-3">Sign Up</button>
            </form>
        </div>
        <div class="text-center mt-3">
            <span>Already have an account? <a href="login.html" target="_blank" class="text-decoration-none link">Login</a></span>
        </div>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```


# OUTPUT:
![3](https://github.com/user-attachments/assets/564e2ebe-bc42-41e8-9bb1-6afc430f5ec6)
![1](https://github.com/user-attachments/assets/0571dad6-c2a7-43d3-974f-67896d5b70a2)
![2](https://github.com/user-attachments/assets/c2d1b8fd-9b61-4744-91fc-668d70f709c1)


# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
