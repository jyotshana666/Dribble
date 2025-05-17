# Project Responsive Web Design using Bootstrap
## Date: 17.05.2025

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
#### home.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Apple</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap" rel="stylesheet">

  <style>
    /* Reset and Fonts */
    body {
      margin: 0;
      font-family: 'Outfit', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }

    /* Hero Section with Fullscreen Video */
    .hero-section {
      position: relative;
      height: 100vh;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
    }

    .hero-video {
      position: absolute;
      top: 50%;
      left: 50%;
      width: 100%;
      height: 100%;
      object-fit: cover;
      transform: translate(-50%, -50%);
      z-index: -1;
    }

    .hero-content {
      z-index: 2;
      color: white;
      background: rgba(0, 0, 0, 0.5);
      padding: 2rem;
      border-radius: 15px;
      max-width: 90%;
    }

    .hero-content h1 {
      font-size: 3rem;
      font-weight: 700;
    }

    .hero-content p {
      font-size: 1.25rem;
      margin-bottom: 1rem;
    }

    .products img {
      height: 300px;
      object-fit: cover;
    }

    footer {
      background-color: #000;
      color: #fff;
      padding: 20px 0;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand" href="#">Apple</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="mac.html">Mac</a></li>
          <li class="nav-item"><a class="nav-link" href="iphone.html">iPhone</a></li>
          <li class="nav-item"><a class="nav-link" href="ipad.html">iPad</a></li>
          <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <header class="hero-section">
    <video autoplay muted loop playsinline class="hero-video">
      <source src="bg.mp4" type="video/mp4" />
    </video>
    <div class="hero-content">
      <h1>iPhone 15 Pro</h1>
      <p>Experience the future in your hand.</p>
      <a href="iphone.html" class="btn btn-light">Learn More</a>
    </div>
  </header>

  <!-- Products Section -->
  <section class="products py-5">
    <div class="container">
      <h2 class="text-center mb-5 fw-bold">Featured Products</h2>
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="macbook_home.jpg" class="card-img-top" alt="MacBook Air">
            <div class="card-body">
              <h5 class="card-title fw-bold">MacBook Air</h5>
              <p class="card-text">Supercharged by M3.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="ipad_home.jpg" class="card-img-top" alt="iPad Air">
            <div class="card-body">
              <h5 class="card-title fw-bold">iPad Air</h5>
              <p class="card-text">Now with M2 chip.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="apple watch_home.jpg" class="card-img-top" alt="iPhone 15 Pro">
            <div class="card-body">
              <h5 class="card-title fw-bold">iPhone 15 Pro</h5>
              <p class="card-text">Titanium. So strong. So light. So Pro.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="text-center">
    <p class="mb-0">© 2025 Apple Clone. Designed for educational purposes.</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```
#### mac.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Mac | Apple </title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap" rel="stylesheet"/>

  <style>
    body {
      margin: 0;
      font-family: 'Outfit', sans-serif;
    }

    /* Hero Section with Background Video */
    .hero-section {
      position: relative;
      height: 100vh;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
    }

    .hero-video {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: -1;
    }

    .hero-content {
      position: relative;
      z-index: 1;
      background: rgba(0, 0, 0, 0.5);
      padding: 2rem;
      border-radius: 12px;
    }

    .hero-content h1 {
      font-size: 3.5rem;
      font-weight: 700;
    }

    .products img {
      height: 250px;
      object-fit: cover;
      border-radius: 8px 8px 0 0;
    }

    .card {
      transition: transform 0.3s ease;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    footer {
      background-color: #000;
      color: #fff;
      padding: 20px 0;
      font-size: 0.95rem;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="index.html">Apple</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link active" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link active" href="mac.html">Mac</a></li>
          <li class="nav-item"><a class="nav-link" href="iphone.html">iPhone</a></li>
          <li class="nav-item"><a class="nav-link" href="ipad.html">iPad</a></li>
          <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section with Background Video -->
  <header class="hero-section">
    <video autoplay muted loop playsinline class="hero-video">
      <source src="mac_bg.mp4" type="video/mp4" />
    </video>
    <div class="hero-content">
      <h1>MacBook Air</h1>
      <p>Supercharged by the M3 chip</p>
      <a href="mac.html" class="btn btn-light mt-3">Learn More</a>
    </div>
  </header>

  <!-- Product Section -->
  <section class="products py-5">
    <div class="container">
      <h2 class="text-center mb-5 fw-bold">Mac Lineup</h2>
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="macbookair.jpg" class="card-img-top" alt="MacBook Air">
            <div class="card-body">
              <h5 class="card-title fw-bold">MacBook Air 13”</h5>
              <p class="card-text">Lightweight. Fast. Reliable.</p>
              <p class="text-muted fw-semibold">$999</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="mac16.jpg" class="card-img-top" alt="MacBook Pro">
            <div class="card-body">
              <h5 class="card-title fw-bold">MacBook Pro 16”</h5>
              <p class="card-text">Built for power users.</p>
              <p class="text-muted fw-semibold">$2,499</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="imac24.jpg" class="card-img-top" alt="iMac">
            <div class="card-body">
              <h5 class="card-title fw-bold">iMac 24”</h5>
              <p class="card-text">All-in-one desktop with M3.</p>
              <p class="text-muted fw-semibold">$1,299</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

<!-- Mac Features Section -->
<section class="features py-5 bg-light">
  <div class="container">
    <h2 class="text-center fw-bold mb-5">Why Mac?</h2>
    <div class="row g-4">
      <div class="col-md-4 text-center">
        <img src="https://img.icons8.com/ios-filled/100/000000/rocket--v1.png" alt="Performance Icon" width="60" />
        <h5 class="mt-3 fw-semibold">Lightning Performance</h5>
        <p>Experience blazing speed with the Apple Silicon chips designed for pro-level work and play.</p>
      </div>
      <div class="col-md-4 text-center">
        <img src="https://img.icons8.com/ios-filled/100/000000/security-checked.png" alt="Security Icon" width="60" />
        <h5 class="mt-3 fw-semibold">Built-In Security</h5>
        <p>With built-in security features and seamless updates, your data stays protected and private.</p>
      </div>
      <div class="col-md-4 text-center">
        <img src="https://img.icons8.com/ios-filled/100/000000/mac-os.png" alt="macOS Icon" width="60" />
        <h5 class="mt-3 fw-semibold">macOS Experience</h5>
        <p>Intuitive, beautiful, and powerful. macOS makes it easy to get things done — your way.</p>
      </div>
    </div>
  </div>
</section>

<!-- Footer -->
<footer class="text-center mt-5">
  <p class="mb-0">© 2025 Apple Clone | Mac Page | Educational Use</p>
</footer>

<!-- Bootstrap JS -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>


```
#### ipad.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>iPad | Apple </title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap" rel="stylesheet"/>

  <style>
    body {
      margin: 0;
      font-family: 'Outfit', sans-serif;
    }

    .hero-section {
      position: relative;
      height: 100vh;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
    }

    .hero-video {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: -1;
    }

    .hero-content {
      position: relative;
      z-index: 1;
      background: rgba(0, 0, 0, 0.5);
      padding: 2rem;
      border-radius: 12px;
    }

    .hero-content h1 {
      font-size: 3.5rem;
      font-weight: 700;
    }

    .products img {
      height: 250px;
      object-fit: cover;
      border-radius: 8px 8px 0 0;
    }

    .card {
      transition: transform 0.3s ease;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    footer {
      background-color: #000;
      color: #fff;
      padding: 20px 0;
      font-size: 0.95rem;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="index.html">Apple</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="mac.html">Mac</a></li>
          <li class="nav-item"><a class="nav-link" href="index.html">iPhone</a></li>
          <li class="nav-item"><a class="nav-link active" href="ipad.html">iPad</a></li>
          <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section with Background Video -->
  <header class="hero-section">
    <video autoplay muted loop playsinline class="hero-video">
      <source src="ipad bg.mp4" type="video/mp4" />
    </video>
    <div class="hero-content">
      <h1>iPad Pro</h1>
      <p>Supercharged by the Apple M4 chip</p>
      <a href="#" class="btn btn-light mt-3">Learn More</a>
    </div>
  </header>

  <!-- Product Section -->
  <section class="products py-5">
    <div class="container">
      <h2 class="text-center mb-5 fw-bold">iPad Lineup</h2>
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="ipad_home.jpg" class="card-img-top" alt="iPad Pro">
            <div class="card-body">
              <h5 class="card-title fw-bold">iPad Pro 12.9”</h5>
              <p class="card-text">The ultimate iPad experience with M4 chip.</p>
              <p class="text-muted fw-semibold">$1,199</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="ipad pro.jpg" class="card-img-top" alt="iPad Air">
            <div class="card-body">
              <h5 class="card-title fw-bold">iPad Air</h5>
              <p class="card-text">Light. Bright. Powerful.</p>
              <p class="text-muted fw-semibold">$599</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="ipad 10.jpg" class="card-img-top" alt="iPad 10th Gen">
            <div class="card-body">
              <h5 class="card-title fw-bold">iPad 10th Gen</h5>
              <p class="card-text">Colorful, fun, and affordable.</p>
              <p class="text-muted fw-semibold">$449</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

<!-- iPad Features Section -->
<section class="features py-5 bg-light">
  <div class="container">
    <h2 class="text-center fw-bold mb-5">Why iPad?</h2>
    <div class="row g-4">
      <div class="col-md-4 text-center">
        <img src="https://img.icons8.com/ios-filled/100/000000/tablet.png" alt="Performance Icon" width="60" />
        <h5 class="mt-3 fw-semibold">Powerful & Portable</h5>
        <p>The power of a computer in a portable, thin design. Get things done anywhere.</p>
      </div>
      <div class="col-md-4 text-center">
        <img src="https://img.icons8.com/ios-filled/100/000000/drawing.png" alt="Pencil Icon" width="60" />
        <h5 class="mt-3 fw-semibold">Apple Pencil Support</h5>
        <p>Take notes, draw, and create with precision using Apple Pencil (2nd Gen & USB-C).</p>
      </div>
      <div class="col-md-4 text-center">
        <img src="https://img.icons8.com/ios-filled/100/000000/multitasking.png" alt="Multitasking Icon" width="60" />
        <h5 class="mt-3 fw-semibold">Multitask Like a Pro</h5>
        <p>Use Split View and Stage Manager to boost productivity across apps and tasks.</p>
      </div>
    </div>
  </div>
</section>

<!-- Footer -->
<footer class="text-center mt-5">
  <p class="mb-0">© 2025 Apple Clone | iPad Page | Educational Use</p>
</footer>

<!-- Bootstrap JS -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```
#### iphone.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>iPhone | Apple </title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap" rel="stylesheet"/>

  <style>
    body {
      margin: 0;
      font-family: 'Outfit', sans-serif;
    }

    .hero-section {
      position: relative;
      height: 100vh;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
    }

    .hero-video {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: -1;
    }

    .hero-content {
      position: relative;
      z-index: 1;
      background: rgba(0, 0, 0, 0.5);
      padding: 2rem;
      border-radius: 12px;
    }

    .hero-content h1 {
      font-size: 3.5rem;
      font-weight: 700;
    }

    .products img {
      height: 250px;
      object-fit: cover;
      border-radius: 8px 8px 0 0;
    }

    .card {
      transition: transform 0.3s ease;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    footer {
      background-color: #000;
      color: #fff;
      padding: 20px 0;
      font-size: 0.95rem;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="index.html">Apple</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="mac.html">Mac</a></li>
          <li class="nav-item"><a class="nav-link active" href="iphone.html">iPhone</a></li>
          <li class="nav-item"><a class="nav-link" href="ipad.html">iPad</a></li>
          <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section with Background Video -->
  <header class="hero-section">
    <video autoplay muted loop playsinline class="hero-video">
      <source src="iphone bg.mp4" type="video/mp4" />
    </video>
    <div class="hero-content">
      <h1>iPhone 15 Pro</h1>
      <p>Titanium. So strong. So light. So Pro.</p>
      <a href="#" class="btn btn-light mt-3">Learn More</a>
    </div>
  </header>

  <!-- Product Section -->
  <section class="products py-5">
    <div class="container">
      <h2 class="text-center mb-5 fw-bold">iPhone Lineup</h2>
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="iphon15.jpg" class="card-img-top" alt="iPhone 15">
            <div class="card-body">
              <h5 class="card-title fw-bold">iPhone 15</h5>
              <p class="card-text">Dynamic Island. All-day battery life.</p>
              <p class="text-muted fw-semibold">$799</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="iphone 15 pro.jpg" class="card-img-top" alt="iPhone 15 Pro">
            <div class="card-body">
              <h5 class="card-title fw-bold">iPhone 15 Pro</h5>
              <p class="card-text">Pro camera system. A17 Pro chip.</p>
              <p class="text-muted fw-semibold">$999</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="iphone 14.jpg" class="card-img-top" alt="iPhone 14">
            <div class="card-body">
              <h5 class="card-title fw-bold">iPhone 14</h5>
              <p class="card-text">Tried and tested. Still powerful.</p>
              <p class="text-muted fw-semibold">$699</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

<!-- iPhone Features Section -->
<section class="features py-5 bg-light">
  <div class="container">
    <h2 class="text-center fw-bold mb-5">Why iPhone?</h2>
    <div class="row g-4">
      <div class="col-md-4 text-center">
        <img src="https://img.icons8.com/ios-filled/100/000000/smartphone-ram.png" alt="Performance Icon" width="60" />
        <h5 class="mt-3 fw-semibold">Blazing Performance</h5>
        <p>The A17 Pro chip brings console-level gaming and unmatched speed to your pocket.</p>
      </div>
      <div class="col-md-4 text-center">
        <img src="https://img.icons8.com/ios-filled/100/000000/privacy.png" alt="Privacy Icon" width="60" />
        <h5 class="mt-3 fw-semibold">Privacy First</h5>
        <p>Built with privacy at its core, your data stays safe with every interaction.</p>
      </div>
      <div class="col-md-4 text-center">
        <img src="https://img.icons8.com/ios-filled/100/000000/camera.png" alt="Camera Icon" width="60" />
        <h5 class="mt-3 fw-semibold">Pro-Grade Cameras</h5>
        <p>Take studio-quality photos and videos with the advanced camera systems on iPhone.</p>
      </div>
    </div>
  </div>
</section>

<!-- Footer -->
<footer class="text-center mt-5">
  <p class="mb-0">© 2025 Apple Clone | iPhone Page | Educational Use</p>
</footer>

<!-- Bootstrap JS -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```
#### contact.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Apple Support</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css" rel="stylesheet"/>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #f8f9fa;
      scroll-behavior: smooth;
    }

    header {
      background: linear-gradient(135deg, #000, #333);
      color: white;
      padding: 80px 0;
      text-align: center;
    }

    .support-icons i {
      font-size: 2.5rem;
      color: #0d6efd;
    }

    .support-icons h5 {
      margin-top: 1rem;
      font-weight: 600;
    }

    .card-hover:hover {
      transform: translateY(-5px);
      transition: all 0.3s ease-in-out;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
    }

    .form-section {
      background: white;
      border-radius: 12px;
      box-shadow: 0 0 20px rgba(0, 0, 0, 0.05);
      padding: 2rem;
    }

    footer {
      background-color: #000;
      color: white;
      padding: 20px 0;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="#">AppleSupport</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navMenu">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navMenu">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <a class="nav-link active" href="home.html">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#devices">Devices</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#feedback">Feedback</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Header -->
  <header id="home">
    <div class="container">
      <h1 class="display-5 fw-bold">Contact Apple Support</h1>
      <p class="lead">Help for iPad, iPhone, Mac and more</p>
    </div>
  </header>

  <!-- Support Options -->
  <section id="devices" class="py-5">
    <div class="container">
      <h2 class="text-center fw-bold mb-4">Get Help For Your Devices</h2>
      <div class="row text-center g-4 support-icons">
        <div class="col-6 col-md-4 col-lg-2">
          <div class="card p-3 border-0 card-hover">
            <i class="bi bi-phone"></i>
            <h5>iPhone</h5>
          </div>
        </div>
        <div class="col-6 col-md-4 col-lg-2">
          <div class="card p-3 border-0 card-hover">
            <i class="bi bi-laptop"></i>
            <h5>Mac</h5>
          </div>
        </div>
        <div class="col-6 col-md-4 col-lg-2">
          <div class="card p-3 border-0 card-hover">
            <i class="bi bi-tablet"></i>
            <h5>iPad</h5>
          </div>
        </div>
        <div class="col-6 col-md-4 col-lg-2">
          <div class="card p-3 border-0 card-hover">
            <i class="bi bi-person-circle"></i>
            <h5>Account</h5>
          </div>
        </div>
        <div class="col-6 col-md-4 col-lg-2">
          <div class="card p-3 border-0 card-hover">
            <i class="bi bi-shop"></i>
            <h5>App Store</h5>
          </div>
        </div>
        <div class="col-6 col-md-4 col-lg-2">
          <div class="card p-3 border-0 card-hover">
            <i class="bi bi-three-dots"></i>
            <h5>More</h5>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Feedback Form -->
  <section id="feedback" class="py-5 bg-light">
    <div class="container">
      <div class="form-section mx-auto" style="max-width: 700px;">
        <h3 class="mb-4 text-center fw-semibold">Send Us Your Feedback</h3>
        <form>
          <div class="form-floating mb-3">
            <input type="text" class="form-control" id="nameInput" placeholder="Your Name" required>
            <label for="nameInput">Your Name</label>
          </div>
          <div class="form-floating mb-3">
            <input type="email" class="form-control" id="emailInput" placeholder="name@example.com" required>
            <label for="emailInput">Email address</label>
          </div>
          <div class="form-floating mb-3">
            <select class="form-select" id="categorySelect">
              <option selected>Choose a category</option>
              <option value="ipad">iPad</option>
              <option value="iphone">iPhone</option>
              <option value="mac">Mac</option>
              <option value="appstore">App Store</option>
              <option value="other">Other</option>
            </select>
            <label for="categorySelect">Feedback Category</label>
          </div>
          <div class="form-floating mb-3">
            <textarea class="form-control" placeholder="Leave a message here" id="messageTextarea" style="height: 120px" required></textarea>
            <label for="messageTextarea">Your Message</label>
          </div>
          <div class="text-center">
            <button class="btn btn-primary px-4" type="submit">Submit Feedback</button>
          </div>
        </form>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="text-center">
    <p class="mb-0">© 2025 Apple Clone | Support Page | Educational Use Only</p>
  </footer>

  <!-- Bootstrap JS -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```

## OUTPUT:
### home.html
![alt text](<Screenshot 2025-05-17 201034.png>)
### mac.html
![alt text](<Screenshot 2025-05-17 201040.png>)
### ipad.html
![alt text](<Screenshot 2025-05-17 201046.png>)
### iphone.html
![alt text](<Screenshot 2025-05-17 201052.png>)
### contact.html
![alt text](<Screenshot 2025-05-17 201133.png>)


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
