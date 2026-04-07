# static-website-azure-blob
Hosting first Static Website with Azure
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Azure Blob Static Site</title>
  <meta name="description" content="A fancy static website hosted in Microsoft Azure Blob Storage." />
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="stars"></div>
  <div class="glow glow-1"></div>
  <div class="glow glow-2"></div>

  <header class="hero">
    <nav class="nav">
      <div class="logo">☁ Azure Blob Site</div>
      <a class="nav-btn" href="#learn">Learn More</a>
    </nav>

    <section class="hero-content">
      <p class="tag">Static website • GitHub repo • Azure Blob</p>
      <h1>
        You did it.<br />
        <span>Welcome to your fancy Azure static website.</span>
      </h1>
      <p class="subtext">
        This site is made with plain HTML, CSS, and JavaScript so it is easy to upload
        to Azure Blob Storage and easy to understand.
      </p>

      <div class="hero-buttons">
        <a href="#cards" class="btn btn-primary">See the magic</a>
        <a href="#steps" class="btn btn-secondary">Simple steps</a>
      </div>
    </section>
  </header>

  <main>
    <section id="cards" class="cards-section">
      <div class="section-title">
        <h2>Why this is cool</h2>
        <p>It looks nice, but it is still simple.</p>
      </div>

      <div class="cards">
        <article class="card">
          <div class="card-icon">⚡</div>
          <h3>Fast</h3>
          <p>Static sites load quickly because there is no big server doing extra work.</p>
        </article>

        <article class="card">
          <div class="card-icon">🧠</div>
          <h3>Easy</h3>
          <p>Only a few files. That means less confusion and easier fixing later.</p>
        </article>

        <article class="card">
          <div class="card-icon">☁</div>
          <h3>Azure Ready</h3>
          <p>Perfect for uploading into Azure Blob Storage static website hosting.</p>
        </article>
      </div>
    </section>

    <section id="learn" class="highlight">
      <div class="highlight-box">
        <h2>Your website can live in the cloud</h2>
        <p>
          Put these files in Azure, and people can visit your site from a web link.
        </p>
        <button id="funButton" class="btn btn-primary">Press me</button>
        <p id="funMessage" class="fun-message"></p>
      </div>
    </section>

    <section id="steps" class="steps-section">
      <div class="section-title">
        <h2>Super simple idea</h2>
        <p>Think of it like putting drawings into a magic online folder.</p>
      </div>

      <div class="steps">
        <div class="step">
          <span>1</span>
          <p>Make your website files.</p>
        </div>
        <div class="step">
          <span>2</span>
          <p>Turn on Static Website in Azure.</p>
        </div>
        <div class="step">
          <span>3</span>
          <p>Upload files to the cloud.</p>
        </div>
        <div class="step">
          <span>4</span>
          <p>Open your link and smile.</p>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <p>Made for Azure Blob Static Website hosting ✨</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
