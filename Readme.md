## Create index.html

```
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bootstrap Tutorial</title>
</head>
<body>
  
</body>
</html>
```

## Add Bootstrap Library

Head to the [Bootstrap Getting Started page](https://getbootstrap.com/docs/5.1/getting-started/introduction/) for more details.

### CSS

Copy-paste the stylesheet <link> into your <head> before all other stylesheets to load our CSS.

```
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-F3w7mX95PdgyTmZZMECAngseQB83DfGTowi0iMjiWaeVhAn4FJkqJByhZMI3AhiU" crossorigin="anonymous">
```

### JS

Copy-paste the script <script> into your <head>

```
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.1/dist/js/bootstrap.bundle.min.js" integrity="sha384-/bQdsTh/da6pkI1MST/rWKFNjaCP5gBSY4sEBT38Q/9RBh9AH40zEOg7Hlq2THRZ" crossorigin="anonymous"></script>
```

## Create a [Container](https://getbootstrap.com/docs/5.1/layout/containers/)

Add the html below into the `<body>` tag

```
<div class="container">
  <div class="row">
  </div>
</div>
```

## Create a Nav

Add the html below into the `<div class="row">` tag

```
<ul class="nav">
  <li class="nav-item">
    <a class="nav-link active" aria-current="page" href="#">Home</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">About</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">Contact</a>
  </li>
</ul>
```

## Create a [Carousel](https://getbootstrap.com/docs/5.1/components/carousel/)

Play around with updating the `src` attribute on the `<img>` tag

```
<div id="main-carousel" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="https://images.unsplash.com/photo-1605457867610-e990b192418e?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1100&q=80" class="d-block w-100" alt="">
    </div>
    <div class="carousel-item">
      <img src="https://images.unsplash.com/photo-1561424412-6c2125ecb1cc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2000&q=80" class="d-block w-100" alt="">
    </div>
    <div class="carousel-item">
      <img src="https://images.unsplash.com/photo-1616070152767-3eb99cf10509?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2000&q=80" class="d-block w-100" alt="">
    </div>
  </div>
</div>
```

## Add About Section with [Cards](https://getbootstrap.com/docs/5.1/components/card/)

```
<section id="about">
  <h1>About</h1>

  <div class="col">
    <div class="card">
      <img
        src="https://images.unsplash.com/photo-1511283402428-355853756676?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1100&q=80"
        class="card-img-top" alt="">
      <div class="card-body">
        <h5 class="card-title">Card title</h5>
        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's
          content.</p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
      </div>
    </div>
  </div>

  <div class="col">
    <div class="card">
      <img
        src="https://images.unsplash.com/photo-1520640023173-50a135e35804?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1100&q=80"
        class="card-img-top" alt="">
      <div class="card-body">
        <h5 class="card-title">Card title</h5>
        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's
          content.</p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
      </div>
    </div>
  </div>

  <div class="col">
    <div class="card">
      <img
        src="https://images.unsplash.com/photo-1573920372704-3b46ad13f5f9?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1100&q=80"
        class="card-img-top" alt="">
      <div class="card-body">
        <h5 class="card-title">Card title</h5>
        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's
          content.</p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
      </div>
    </div>
  </div>
</section>
```

### Add Margin Below Carousel

The about section feels a little too close to the carousel.  To fix we can use Bootstrap's [spacing utilities](https://getbootstrap.com/docs/5.1/utilities/spacing/) to add some margin to the bottom of the carousel.

Add the `mb-5` class to the carousel.

## Add Contact Section

### Add [Form](https://getbootstrap.com/docs/5.1/forms/overview/)

```
<form>
  <div class="mb-3">
    <label for="email" class="form-label">Email address</label>
    <input type="email" class="form-control" id="email" aria-describedby="emailHelp" required>
    <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
  </div>
  <label for="source" class="form-label">How did you hear about us</label>
  <div class="mb-3">
    <select id="source" class="form-select" aria-label="How did you hear about us">
      <option selected></option>
      <option value="1">Friend</option>
      <option value="2">Google</option>
      <option value="3">Other</option>
    </select>
  </div>
  <div class="mb-3 form-check">
    <input type="checkbox" class="form-check-input" id="newsletter-check">
    <label class="form-check-label" for="newsletter-check">Sign me up for newsletter</label>
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>
```