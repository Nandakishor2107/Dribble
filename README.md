# Project Responsive Web Design using Bootstrap
## Date:27-12-2024

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :

```
<html>
<head>
  <title>Dribbble</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
  <style>
    .bg-warning {
      background-color: yellow !important;
    }
    .bg-success {
      background-color: lightgreen !important;
    }
    .bg-dark {
      background-color: black !important;
    }
    .text-white {
      color: white !important;
    }
    .text-center {
      text-align: center !important;
    }
    .py-5 {
      padding: 3rem 0 !important;
    }
    .py-3 {
      padding: 1rem 0 !important;
    }
    .navbar {
      padding-left: 0 !important;
    }
    .navbar-brand {
      display: flex;
      align-items: center;
      padding: 0;
    }
    .navbar-brand img {
      width: 100px; 
      height: auto;
      margin-right: 10px; 
    }
    .navbar-brand span {
      font-size: 2rem; 
      font-weight: bold;
      letter-spacing: 2px;
      text-transform: uppercase; 
    }
  </style>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
  <nav class="navbar navbar-expand-lg navbar-light bg-success">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img src="logo.png" alt="Logo">
        <span>dribbble</span>
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navgo">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navgo">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#designs">Designs</a></li>
          <li class="nav-item">
            <a class="nav-link" href="#" data-bs-toggle="modal" data-bs-target="#loginpop">Login</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#" data-bs-toggle="modal" data-bs-target="#signuppop">Sign up</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <div class="modal fade" id="signuppop" tabindex="-1" aria-labelledby="signuppopLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="signuppopLabel">Sign up</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          <form>
            <div class="mb-3">
              <label for="signupname" class="form-label">Name</label>
              <input type="text" class="form-control" id="signupname" placeholder="Enter your Name">
            </div>
            <div class="mb-3">
              <label for="signupmail" class="form-label">E-mail</label>
              <input type="email" class="form-control" id="signupmail" placeholder="Enter your E-mail">
            </div>
            <div class="mb-3">
              <label for="signuppwd" class="form-label">Password</label>
              <input type="password" class="form-control" id="signuppwd" placeholder="Enter your Password">
            </div>
            <button type="submit" class="btn btn-primary w-100">Sign up</button>
          </form>
        </div>
      </div>
    </div>
  </div>

  <div class="modal fade" id="loginpop" tabindex="-1" aria-labelledby="loginpopLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="loginpopLabel">Login</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          <form>
            <div class="mb-3">
              <label for="loginmail" class="form-label">E-mail</label>
              <input type="email" class="form-control" id="loginmail" placeholder="Enter your E-mail">
            </div>
            <div class="mb-3">
              <label for="loginpswd" class="form-label">Password</label>
              <input type="password" class="form-control" id="loginpswd" placeholder="Enter your Password">
            </div>
            <button type="submit" class="btn btn-primary w-100">Login</button>
          </form>
        </div>
      </div>
    </div>
  </div>

  <div class="bg-warning text-center py-5">
    <h1>Welcome to DRIBBLE</h1>
    <p>Place to display your graphic designing skills</p>
  </div>

  <div id="designs" class="container my-5">
    <h2 class="text-center mb-4">Sample works</h2>
    <div class="row">
      <div class="col-md-4 mb-3">
        <div class="card bg-dark text-white">
          <img src="image1.jpg" class="card-img-top" alt="design 1">
          <div class="card-body">
            <h5 class="card-title">Design 1</h5>
            <p class="card-text">Geometry conveyed in its truest form</p>
          </div>
        </div>
      </div>
      <div class="col-md-4 mb-3">
        <div class="card bg-dark text-white">
          <img src="image2.jpg" class="card-img-top" alt="design 2">
          <div class="card-body">
            <h5 class="card-title">Design 2</h5>
            <p class="card-text">Low poly design of deer</p>
          </div>
        </div>
      </div>
      <div class="col-md-4 mb-3">
        <div class="card bg-dark text-white">
          <img src="image3.jpg" class="card-img-top" alt="design 3">
          <div class="card-body">
            <h5 class="card-title">Design 3</h5>
            <p class="card-text">Abstract art involving conspiracies</p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <footer class="bg-dark text-white text-center py-3">
    <p>Designed by Nanda Kishor S P</p>
  </footer>
</body>
</html>

```

## OUTPUT:

![alt text](<Screenshot (118).png>) 

![alt text](<Screenshot (116).png>) 

![alt text](<Screenshot (117).png>)

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
