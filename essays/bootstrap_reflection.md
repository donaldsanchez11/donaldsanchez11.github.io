---
layout: essay
type: essay
title: "Strap your boots! Time for Bootstrap!"
# All dates must be YYYY-MM-DD format!
date: 2026-09-09
published: true
labels:
  - Reflections
  - HTML
  - CSS
  - Bootstrap
---

<figure>
  <img class="img-fluid"
       style="max-width: 600px;"
       src="../img/e10_typescript_reflection/volodymyr-dobrovolskyy-KrYbarbAx5s-unsplash.jpg">

  <figcaption>
    <small>
      Photo by
      <a href="https://unsplash.com/@vladimir_d?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">
        Volodymyr Dobrovolskyy
      </a>
      on
      <a href="https://unsplash.com/photos/a-cat-sitting-in-front-of-a-computer-monitor-KrYbarbAx5s?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">
        Unsplash
      </a>
    </small>
  </figcaption>
</figure>

# Strap your boots! Time for Bootstrap!

## Why bother to use something like Bootstrap 5?

If you don't want to write a bunch of CSS code, Bootstrap 5 is useful. It provides ready-made styles and components, so you don't have to build everything from scratch.

## What does one get in return for the investment of time and frustration?

You have to spend some time learning Bootstrap classes, but in return, you can write fewer lines of CSS and keep your code cleaner. It can also make building websites faster once you understand how it works.

## Why not just use raw HTML and CSS?

If you want more control over your website and want to be more specific with your design, raw HTML and CSS might be better. Bootstrap is useful for saving time, but sometimes its default styles can get in the way.

### HTML without Bootstrap 5
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Website</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <nav class="navbar">
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </nav>

  <div class="container">
    <h1>Welcome to My Website</h1>
    <p>This is my first webpage.</p>
    <button class="button">Click Me</button>
  </div>

</body>
</html>
```

```
body {
  margin: 0;
  font-family: Arial, sans-serif;
}

.navbar {
  background-color: #212529;
  display: flex;
  justify-content: space-around;
  padding: 15px;
}

.navbar a {
  color: white;
  text-decoration: none;
}

.container {
  max-width: 1140px;
  margin: auto;
  padding: 30px 12px;
}

.button {
  background-color: #0d6efd;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 6px;
  cursor: pointer;
}
```
### HTML with Bootstrap 5

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Website</title>

  <link
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
    rel="stylesheet">
</head>
<body>

  <nav class="bg-dark d-flex justify-content-around p-3">
    <a href="#" class="text-white text-decoration-none">Home</a>
    <a href="#" class="text-white text-decoration-none">About</a>
    <a href="#" class="text-white text-decoration-none">Contact</a>
  </nav>

  <div class="container py-4">
    <h1>Welcome to My Website</h1>
    <p>This is my first webpage.</p>
    <button class="btn btn-primary">Click Me</button>
  </div>

</body>
</html>
```

```CSS
/*NOTHING*/
```
## Are there software engineering benefits of UI frameworks?

We software engineers always argue about which system is better. "Python this, Python that," or "Java this, Java that." However, whatever floats your boat is what matters.

The same goes for UI frameworks. If you want to use raw HTML and CSS, go ahead! Just make sure your team agrees with your decision. Changing frameworks out of nowhere can create confusion and unnecessary work for everyone.

In the end, I think the most important thing is choosing the right tool for the project and making sure everyone on the team understands how to use it.
