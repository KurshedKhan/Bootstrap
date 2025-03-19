# Bootstrap Introduction (Basic to Advance)

## What is Bootstrap?
Bootstrap is a popular front-end framework for developing responsive and mobile-first websites. It includes CSS and JavaScript-based design templates for typography, forms, buttons, navigation, and other interface components.

## Key Features
- Responsive Grid System
- Pre-styled Components
- JavaScript Plugins
- Customizable
- Mobile-First Approach

## Getting Started

### 1. Include Bootstrap via CDN
```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
```

### 2. Install via npm
```sh
npm install bootstrap
```

### 3. Basic Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap Example</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <div class="container">
        <h1 class="text-primary">Hello, Bootstrap!</h1>
    </div>
</body>
</html>
```

## Bootstrap Grid System
Bootstrap uses a 12-column grid system.

```html
<div class="container">
    <div class="row">
        <div class="col-md-6 bg-primary text-white">Column 1</div>
        <div class="col-md-6 bg-secondary text-white">Column 2</div>
    </div>
</div>
```

## Bootstrap Components

### 1. Buttons
```html
<button class="btn btn-primary">Primary Button</button>
<button class="btn btn-success">Success Button</button>
```

### 2. Forms
```html
<form>
    <div class="mb-3">
        <label class="form-label">Email</label>
        <input type="email" class="form-control" placeholder="Enter email">
    </div>
</form>
```

### 3. Navbar
```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container-fluid">
        <a class="navbar-brand" href="#">My Website</a>
    </div>
</nav>
```

## Bootstrap JavaScript Components
Bootstrap comes with built-in JavaScript components like modals, tooltips, and carousels.

### 1. Modal
```html
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#myModal">
    Open Modal
</button>

<div class="modal fade" id="myModal" tabindex="-1">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title">Modal Title</h5>
                <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
            </div>
            <div class="modal-body">This is a Bootstrap modal.</div>
        </div>
    </div>
</div>
```

### 2. Carousel
```html
<div id="carouselExample" class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-inner">
        <div class="carousel-item active">
            <img src="image1.jpg" class="d-block w-100" alt="Slide 1">
        </div>
        <div class="carousel-item">
            <img src="image2.jpg" class="d-block w-100" alt="Slide 2">
        </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
        <span class="carousel-control-prev-icon"></span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
        <span class="carousel-control-next-icon"></span>
    </button>
</div>
```

## Customizing Bootstrap
Use SASS to customize Bootstrap.
```sh
npm install sass
```
Create a custom `styles.scss` file:
```scss
@import "node_modules/bootstrap/scss/bootstrap";
```
Compile it:
```sh
sass styles.scss styles.css
```

## Conclusion
Bootstrap simplifies front-end development with pre-styled components and a responsive grid system. It is widely used for building modern web applications.
