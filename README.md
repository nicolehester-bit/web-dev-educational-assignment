your-repo-name/
├── index.html
├── page2.html
└── style.css
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Home Page</title>

  <!-- Link to external CSS file -->
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- Header uses an ID selector -->
  <header id="main-header">
    <h1>Welcome to My Website</h1>
    <nav>
      <a href="page2.html">Go to Page 2</a>
    </nav>
  </header>

  <!-- Flexbox container -->
  <section class="container">
    <div class="card">
      <h2>Card One</h2>
      <p>This is the first card.</p>
    </div>

    <div class="card">
      <h2>Card Two</h2>
      <p>This is the second card.</p>
    </div>

    <div class="card">
      <h2>Card Three</h2>
      <p>This is the third card.</p>
    </div>
  </section>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Page Two</title>

  <!-- Same CSS file is reused -->
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <header id="main-header">
    <h1>Page Two</h1>
    <nav>
      <a href="index.html">Back to Home</a>
    </nav>
  </header>

  <section class="content">
    <h2>About This Page</h2>
    <p>
      This page demonstrates reuse of CSS classes and IDs
      across multiple HTML files.
    </p>
  </section>

</body>
</html>
/* =========================
   Tag-based selectors
   ========================= */
body {
  margin: 0;
  font-family: Arial, sans-serif;
}

h1, h2 {
  margin-bottom: 0.5rem;
}

p {
  line-height: 1.5;
}

/* =========================
   ID selector
   ========================= */
#main-header {
  background-color: #333;
  color: white;
  padding: 1rem;
}

#main-header a {
  color: #ffd700;
  text-decoration: none;
  margin-right: 1rem;
}

/* =========================
   Class selectors + Flexbox
   ========================= */
.container {
  display: flex;              /* Flexbox layout */
  justify-content: space-around;
  gap: 1rem;
  padding: 2rem;
}

.card {
  border: 1px solid #ccc;
  padding: 1rem;
  width: 30%;
  background-color: #f9f9f9;
}

/* =========================
   Additional class selector
   ========================= */
.content {
  padding: 2rem;
}
