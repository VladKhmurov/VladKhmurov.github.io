<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Sample Page with Grid and Flex</title>
  <style>
    /* Skip to Main Content Link */
    .skip-link {
      position: absolute;
      top: -40px;
      left: 0;
      background: #000;
      color: #fff;
      padding: 8px;
      z-index: 100;
      text-decoration: none;
    }

    .skip-link:focus {
      top: 0;
    }

    /* Nav Styling */
    nav {
      display: inline-block;
      width: 80%;
      background-color: #ccc;
      padding: 10px;
    }

    nav img {
      width: 10%;
    }

    /* Commented li style */
    /*
    li {
      list-style-type: none;
      margin: 5px;
    }
    */

    /* Grid layout */
    .grid {
      display: grid;
      grid-template-columns: 40% 40%;
      justify-content: space-around;
      align-items: center;
      row-gap: 20px;
      background-color: #f0f0f0;
      padding: 20px;
    }

    .grid img {
      width: 100%;
    }

    /* Flex layout */
    .flex {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      background-color: #e0e0e0;
      padding: 20px;
    }

    .flex div {
      flex: 1 1 45%;
      margin: 10px;
      padding: 10px;
      background-color: #ddd;
    }
  </style>
</head>
<body>

  <a href="#main-content" class="skip-link">Skip to Main Content</a>

  <header>
    <h1>Welcome to the Sample Page</h1>
  </header>

  <nav>
    <img src="https://via.placeholder.com/50" alt="Logo" />
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Parks</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <main id="main-content">
    <section class="grid">
      <img src="https://via.placeholder.com/150" alt="Grid image 1" />
      <img src="https://via.placeholder.com/150" alt="Grid image 2" />
    </section>

    <section class="flex">
      <div>Flex Box 1</div>
      <div>Flex Box 2</div>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Your Website</p>
  </footer>

</body>
</html>
