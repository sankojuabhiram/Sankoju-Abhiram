//portfolio website

//html
<!DOCTYPE html>
<html>
<head>
  <title>My Portfolio</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>My Portfolio</h1>
    <nav>
      <a href="#about">About Me</a>
      <a href="#work">Work Experience</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main>
    <section id="about">
      <h2>About Me</h2>
      <p>I am a software engineer with 5+ years of experience in building and maintaining web applications. I am passionate about using technology to solve real-world problems and create a positive impact on the world.</p>
    </section>

    <section id="work">
      <h2>Work Experience</h2>
      <ul>
        <li>Software Engineer, Google AI (2023 - Present)</li>
        <li>Software Engineer, Acme Corporation (2018 - 2023)</li>
      </ul>
    </section>

    <section id="contact">
      <h2>Contact</h2>
      <p>Email: me@example.com</p>
      <p>Phone: (123) 456-7890</p>
    </section>
  </main>

  <footer>
    <p>Copyright &copy; 2023 My Name</p>
  </footer>
</body>
</html>



//css
body {
  font-family: sans-serif;
  margin: 0;
  padding: 0;
}

header {
  background-color: #f2f2f2;
  padding: 20px;
}

h1 {
  font-size: 2em;
  margin: 0;
}

nav {
  float: right;
}

nav a {
  text-decoration: none;
  color: black;
  padding: 10px;
}

main {
  padding: 20px;
}

section {
  margin-bottom: 20px;
}

h2 {
  font-size: 1.5em;
}

footer {
  background-color: #f2f2f2;
  padding: 20px;
  text-align: center;
}




// temperature converter 
//html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Temperature Converter</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>Temperature Converter</h1>

        <div class="inputs">
            <label for="celsius">Enter Celsius temperature:</label>
            <input type="number" id="celsius" name="celsius">
        </div>

        <div class="buttons">
            <button onclick="convertCelsiusToFahrenheit()">Convert to Fahrenheit</button>
        </div>

        <div class="outputs">
            <label for="fahrenheit">Fahrenheit temperature:</label>
            <input type="number" id="fahrenheit" name="fahrenheit" readonly>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>

//css
body {
    font-family: sans-serif;
}

.container {
    width: 500px;
    margin: 0 auto;
    text-align: center;
    padding: 20px;
    border: 1px solid #ccc;
}

h1 {
    font-size: 24px;
    margin-bottom: 20px;
}

.inputs {
    margin-bottom: 20px;
}

.inputs label {
    display: block;
    margin-bottom: 5px;
}

.inputs input {
    width: 100px;
    padding: 5px;
    border: 1px solid #ccc;
}

.buttons button {
    padding: 10px 20px;
    background-color: #007bff;
    color: #fff;
    border: none;
    cursor: pointer;
}

.outputs {
    margin-top: 20px;
}

.outputs label {
    display: block;
    margin-bottom: 5px;
}

.outputs input {
    width: 100px;
    padding: 5px;
    border: 1px solid #ccc;
}
// javascript 
function convertCelsiusToFahrenheit() {
    const celsiusInput = document.getElementById('celsius');
    const celsius = parseFloat(celsiusInput.value);

    const fahrenheit = celsius * 1.8 + 32;
    const fahrenheitInput = document.getElementById('fahrenheit');
    fahrenheitInput.value = fahrenheit.toFixed(2);
}

// Netflix 
//html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Netflix Homepage</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Netflix</h1>
    <input type="search" placeholder="Search for movies and TV shows">
    <button>Sign In</button>
  </header>

  <main>
    <section class="featured">
      <h2>Featured Movies and TV Shows</h2>
      <div class="carousel">
        <img src="https://images.netflix.com/ca-en/image/50124303/600x337.jpg" alt="Featured movie">
        <img src="https://images.netflix.com/ca-en/image/50136337/600x337.jpg" alt="Featured TV show">
      </div>
    </section>

    <section class="popular">
      <h2>Popular Movies and TV Shows</h2>
      <div class="grid">
        <img src="https://images.netflix.com/ca-en/image/50136337/600x337.jpg" alt="Popular movie">
        <img src="https://images.netflix.com/ca-en/image/50124303/600x337.jpg" alt="Popular TV show">
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; Netflix 2023</p>
  </footer>
</body>
</html>

// css
body {
  margin: 0;
  padding: 0;
  font-family: sans-serif;
  background-color: #000;
}

header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px;
  background-color: #222;
}

h1 {
  color: white;
  font-size: 24px;
}

input {
  width: 300px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  background-color: red;
  color: white;
  padding: 10px;
  border-radius: 5px;
}

main {
  padding: 20px;
}

.featured {
  margin-bottom: 20px;
}

.carousel {
  display: flex;
  overflow-x: scroll;
}

.popular {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-gap: 20px;
}

img {
  max-width: 100%;
  height: auto;
}

footer {
  text-align: center;
  padding: 20px;
  background-color: #222;
  color: white;
}
