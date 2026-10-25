## Assignment 7.4 — Modern Landing Page Header

### `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modern Landing Page</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header class="navbar">
        <h2 class="logo">WebTech</h2>

        <nav>
            <a href="#">Home</a>
            <a href="#">About</a>
            <a href="#">Services</a>
        </nav>

        <a href="#" class="cta">Get Started</a>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>Build Your Future Online</h1>
            <p>Learn modern web development and create amazing websites with us.</p>
            <button>Explore Now</button>
        </div>

        <div class="hero-image">
            <img src="https://placehold.co/500x350?text=Web+Development"
                 alt="Web development illustration">
        </div>
    </section>

    <footer>
        <p>© 2026 WebTech. All rights reserved.</p>
    </footer>

</body>
</html>
```

### `style.css`

```css
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #f4f7fb;
    color: #222;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 8%;
    background: white;
    position: sticky;
    top: 0;
    z-index: 10;
}

.logo {
    color: navy;
}

nav {
    display: flex;
    gap: 25px;
}

nav a {
    text-decoration: none;
    color: #333;
}

.cta, button {
    background: navy;
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 6px;
    text-decoration: none;
    cursor: pointer;
}

.hero {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 40px;
    padding: 70px 8%;
    min-height: 500px;
}

.hero-content {
    flex: 1;
}

.hero-content h1 {
    font-size: 42px;
    color: navy;
}

.hero-content p {
    font-size: 18px;
    line-height: 1.6;
}

.hero-image {
    flex: 1;
}

.hero-image img {
    width: 100%;
    max-width: 500px;
    border-radius: 12px;
}

footer {
    text-align: center;
    padding: 20px;
    background: navy;
    color: white;
}

@media (max-width: 700px) {
    .navbar {
        flex-direction: column;
        gap: 15px;
    }

    nav {
        flex-wrap: wrap;
        justify-content: center;
    }

    .hero {
        flex-direction: column;
        text-align: center;
        padding: 40px 20px;
    }

    .hero-content h1 {
        font-size: 32px;
    }
}
```

**Submission:** Save both files in the same folder and open `index.html` using Live Server. Resize the browser to test the responsive layout.