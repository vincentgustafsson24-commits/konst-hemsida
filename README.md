<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8">
  <title>Vincent Gustafsson</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>VINCENT GUSTAFSSON</h1>
    <nav class="top-menu">
      <a href="index.html" class="active">HOME</a>
      <a href="about.html">ABOUT ME</a>
    </nav>
  </header>

  <aside class="side-menu">
    <a href="index.html" class="active">Gallery</a>
    <a href="something.html">Something else</a>
  </aside>

  <main class="gallery">
    <!-- Exempelbilder (byt src till dina egna bilder) -->
    <a href="artwork1.html"><img src="bilder/bild1.jpg" alt="Artwork 1"></a>
    <a href="artwork2.html"><img src="bilder/bild2.jpg" alt="Artwork 2"></a>
    <a href="artwork3.html"><img src="bilder/bild3.jpg" alt="Artwork 3"></a>
    <a href="artwork4.html"><img src="bilder/bild4.jpg" alt="Artwork 4"></a>
    <a href="artwork5.html"><img src="bilder/bild5.jpg" alt="Artwork 5"></a>
    <a href="artwork6.html"><img src="bilder/bild6.jpg" alt="Artwork 6"></a>
    <!-- fortsätt lägga till fler bilder -->
  </main>
</body>
</html>
<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8">
  <title>About Me - Vincent Gustafsson</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>VINCENT GUSTAFSSON</h1>
    <nav class="top-menu">
      <a href="index.html">HOME</a>
      <a href="about.html" class="active">ABOUT ME</a>
    </nav>
  </header>

  <aside class="side-menu">
    <a href="index.html">Gallery</a>
    <a href="something.html">Something else</a>
  </aside>

  <main class="about">
    <h2>Om mig</h2>
    <p>Hej! Jag heter Vincent Gustafsson och jag målar främst med oljefärg. 
       Här kan du se några bilder på mig när jag målar och läsa lite om mitt arbete.</p>

    <img src="bilder/vincent1.jpg" alt="Vincent målar">
    <img src="bilder/vincent2.jpg" alt="Vincent i ateljén">
  </main>
</body>
</html>
<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8">
  <title>Artwork 1 - Vincent Gustafsson</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>VINCENT GUSTAFSSON</h1>
    <nav class="top-menu">
      <a href="index.html">HOME</a>
      <a href="about.html">ABOUT ME</a>
    </nav>
  </header>

  <main class="artwork-detail">
    <img src="bilder/bild1.jpg" alt="Artwork 1">
    <div class="info">
      <h2>Title: Example</h2>
      <p><strong>Year:</strong> 2025</p>
      <p><strong>Size:</strong> 40x50 cm</p>
      <p><strong>About:</strong> Här kan du skriva en beskrivning om målningen.</p>
    </div>
  </main>
</body>
</html>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: white;
  color: black;
}

/* Header */
header {
  text-align: center;
  padding: 20px 0;
}
header h1 {
  margin: 0;
  font-size: 28px;
  font-weight: bold;
}
.top-menu {
  margin-top: 10px;
}
.top-menu a {
  margin: 0 15px;
  text-decoration: none;
  color: black;
  font-weight: bold;
}
.top-menu a.active {
  text-decoration: underline;
}

/* Side menu */
.side-menu {
  position: fixed;
  top: 120px;
  left: 20px;
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.side-menu a {
  text-decoration: none;
  color: black;
}
.side-menu a.active {
  font-weight: bold;
  text-decoration: underline;
}

/* Gallery grid */
.gallery {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  gap: 15px;
  padding: 50px 80px;
}
.gallery img {
  width: 100%;
  height: auto;
  transition: transform 0.3s;
}
.gallery img:hover {
  transform: scale(1.05);
}

/* About page */
.about {
  padding: 50px 80px;
}
.about img {
  max-width: 300px;
  margin: 20px;
}

/* Artwork detail */
.artwork-detail {
  display: flex;
  gap: 40px;
  padding: 50px 80px;
}
.artwork-detail img {
  max-width: 500px;
  height: auto;
}
.artwork-detail .info {
  max-width: 400px;
}
