# Project Responsive Web Design using Bootstrap
# Date:23-12-2024
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
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />

    <!-- Bootstrap CSS -->
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta2/dist/css/bootstrap.min.css"
      rel="stylesheet"
      integrity="sha384-BmbxuPwQa2lc/FVzBcNJ7UAyJxM6wuqIj61tLrc4wSX0szH/Ev+nYRRuWlolflfl"
      crossorigin="anonymous"
    />
    <link rel="stylesheet" href="style.css" />
    <link rel="preconnect" href="https://fonts.gstatic.com" />
    <link
      href="https://fonts.googleapis.com/css2?family=Roboto+Condensed&display=swap"
      rel="stylesheet"
    />
    <title>Project</title>
    <style>
      * {
        margin: 0;
        padding: 0;
        font-family: 'Roboto Condensed', sans-serif;
      }

      /* Navbar */
      .navbar-nav {
        margin-right: 0 !important;
        padding-right: 100px;
      }

      .navbar {
        background-color: #0a193d;
        color: white !important;
      }

      .nav-item a {
        color: white !important;
      }

      .navbar-brand {
        color: white !important;
        padding-left: 100px;
      }

      /* Banner */
      #banner-container {
        background-color: #0a193d;
        color: white !important;
        padding: 80px 0;
      }

      #banner-row img {
        max-width: 50%;
        height: auto;
        display: block;
        margin: 0 auto;
      }

      #banner-row h3,
      #banner-row p {
        text-align: center;
      }

      #banner-row a {
        background-color: white !important;
        color: black !important;
        border: none;
        margin-top: 20px;
      }

      /* Service Section */
      #service {
        padding: 80px 0;
      }

      #service h1 {
        padding-bottom: 70px;
      }

      /* Ensure all images have equal dimensions */
      .fixed-image {
        width: 200px;
        height: 200px;
        object-fit: cover;
      }

      /* Footer Section */
      #footer {
        background-color: #0a193d;
        color: white;
        padding: 40px 0;
        text-align: center;
      }

      #footer h3 {
        margin-bottom: 15px;
      }

      #footer p {
        margin: 5px 0;
      }

      #footer .col-md-4 {
        display: flex;
        flex-direction: column;
        align-items: center; /* Centers the content horizontally */
        justify-content: center; /* Centers the content vertically */
      }
    </style>
  </head>
  <body>
    <!-- Navbar -->
    <section id="navbar">
      <nav class="navbar navbar-expand-lg navbar-light">
        <div class="container-fluid">
          <a class="navbar-brand" href="#">Dribble</a>
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav m-auto">
              <li class="nav-item">
                <a class="nav-link active" aria-current="page" href="#">Home</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#service">Projects</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#social">Sign In</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </section>

    <!-- Banner -->
    <section id="banner">
      <div class="container-fluid" id="banner-container">
        <div class="row" id="banner-row">
          <img src="fusion.png" alt="Fusion 360 Banner" />
          <div class="col-md-12">
            <br />
            <h3>BEST PROFESSIONAL FUSION 360 DESIGN DEVELOPMENT COMPANY</h3>
            <p>The fastest way to grow your business with the leader in Fusion 360 Autodesk</p>
            <div class="d-grid gap-2 d-md-flex justify-content-center">
              <a class="btn btn-primary" href="#" role="button">Sign In</a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Services -->
    <section id="service">
      <h1 class="text-center">PROJECTS</h1>
      <div class="container-fluid">
        <div class="row">
          <!-- Plumber Block -->
          <div class="col-md-4 d-flex flex-column align-items-center">
            <h3>Plumber Block</h3>
            <img src="pro1.webp" class="img-fluid rounded fixed-image" alt="Plumber Block" />
            <p>
              The plummer block, which is an assembly comprising of a self-aligning ball bearing or spherical roller bearing placed in bearing boxes of various shapes...
            </p>
          </div>

          <!-- Screw Jack -->
          <div class="col-md-4 d-flex flex-column align-items-center">
            <h3>Screw Jack</h3>
            <img src="pro2.png" class="img-fluid rounded fixed-image" alt="Screw Jack" />
            <p>A jackscrew, or screw jack, is a type of jack that is operated by turning a leadscrew...</p>
          </div>

          <!-- Robotic Gripper -->
          <div class="col-md-4 d-flex flex-column align-items-center">
            <h3>Robotic Gripper</h3>
            <img src="pro3.jpg" class="img-fluid rounded fixed-image" alt="Robotic Gripper" />
            <p>Flange coupling is a sort of connector between turning chutes that have two arrangements of flanges...</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <section id="footer">
      <div class="container-fluid">
        <div class="row">
          <div class="col-md-4">
            <h3>Our Website</h3>
            <p>fusion360@gmail.com</p>
          </div>
          <div class="col-md-4">
            <h3>Contact Us</h3>
            <p>Call Us - 1800-121-6532</p>
            <p>Email Us - fusion360@gmail.com</p>
          </div>
          <div class="col-md-4">
            <h3>Sign In Our Website</h3>
            <form action="#" method="post">
              <div class="mb-3">
                <input
                  type="email"
                  placeholder="Enter Your Email"
                  class="form-control"
                  id="exampleInputEmail1"
                  aria-describedby="emailHelp"
                />
                <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
              </div>
              <button type="submit" class="btn btn-primary">Submit</button>
            </form>
          </div>
        </div>
      </div>
    </section>
  </body>
</html>
```
# OUTPUT:
![alt text](<Screenshot (50).png>)
![alt text](<Screenshot (51).png>)
# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
